# Инфраструктура и пайплайн (CI/CD)

Современная автоматизация тестирования неотделима от CI/CD-инфраструктуры. Написанные тесты должны запускаться автоматически при изменении кода, а не вручную на локальной машине — только тогда они обеспечивают быструю обратную связь. Компетентность в настройке пайплайнов стала базовым ожиданием от QA-инженера наравне с умением писать тесты.

## Определение

**Непрерывная интеграция (Continuous Integration, CI)** — практика автоматической проверки каждого изменения кода: сборка, статический анализ, тесты. Цель — выявить проблемы до слияния в основную ветку.

**Непрерывная поставка (Continuous Delivery, CD)** — расширение CI: после успешной проверки артефакт автоматически готов к развёртыванию в любом окружении. При **Continuous Deployment** — деплой в production происходит без ручного подтверждения.

## Инструменты CI/CD

| Инструмент | Статус 2025 | Когда выбирать |
|---|---|---|
| **GitHub Actions** | Стандарт для новых проектов (68% GitHub-проектов) | Проект на GitHub; нужна простая настройка и богатый marketplace |
| **GitLab CI** | Enterprise-стандарт для self-hosted | GitLab-инфраструктура; встроен в платформу без доп. инструментов |
| **Jenkins** | Legacy backbone; 67% команд мигрируют от него | Существующие enterprise-инсталляции; сложные кастомные сценарии |
| **Azure DevOps** | 24% рынка, Microsoft-экосистема | .NET/Azure стек; интеграция с Jira/Teams |
| **CircleCI / TeamCity** | Нишевые enterprise | Специфические требования к hosted-инфраструктуре |

{% hint style="warning" %}
Jenkins остаётся в использовании в крупных enterprise-компаниях с исторически сложившейся инфраструктурой. Для новых проектов выбор по умолчанию — GitHub Actions или GitLab CI.
{% endhint %}

## Современный pipeline: структура stages

Зрелый тестовый пайплайн строится по принципу воронки — быстрые проверки блокируют медленные:

```
commit
  └─► lint / static analysis          (1–2 мин)
        └─► unit tests                (2–5 мин)
              └─► build               (3–10 мин)
                    └─► integration tests           (5–15 мин)
                          └─► E2E (sharded)         (10–20 мин)
                                └─► visual regression  (параллельно с E2E)
                                      └─► contract tests
                                            └─► deploy to staging
```

Каждый этап — отдельный job. Провал любого этапа блокирует продвижение дальше.

### Пример GitHub Actions workflow для Playwright с sharding

```yaml
name: E2E Tests

on:
  push:
    branches: [main, develop]
  pull_request:
    branches: [main]

jobs:
  e2e:
    runs-on: ubuntu-latest
    strategy:
      matrix:
        shard: [1/4, 2/4, 3/4, 4/4]
    steps:
      - uses: actions/checkout@v4

      - uses: actions/setup-node@v4
        with:
          node-version: '20'
          cache: 'npm'

      - name: Install dependencies
        run: npm ci

      - name: Install Playwright browsers
        run: npx playwright install --with-deps chromium

      - name: Run Playwright tests (shard ${{ matrix.shard }})
        run: npx playwright test --shard=${{ matrix.shard }}

      - name: Upload blob report
        if: always()
        uses: actions/upload-artifact@v4
        with:
          name: blob-report-${{ strategy.job-index }}
          path: blob-report/

  merge-reports:
    needs: e2e
    runs-on: ubuntu-latest
    if: always()
    steps:
      - uses: actions/checkout@v4
      - uses: actions/setup-node@v4
        with:
          node-version: '20'
          cache: 'npm'
      - run: npm ci
      - name: Download blob reports
        uses: actions/download-artifact@v4
        with:
          path: all-blob-reports
          pattern: blob-report-*
          merge-multiple: true
      - name: Merge into HTML report
        run: npx playwright merge-reports --reporter html ./all-blob-reports
      - name: Upload HTML report
        uses: actions/upload-artifact@v4
        with:
          name: html-report
          path: playwright-report/
```

### Пример GitLab CI для pytest

```yaml
stages:
  - unit
  - e2e

unit-tests:
  stage: unit
  image: python:3.12
  script:
    - pip install -r requirements.txt
    - pytest tests/unit --junitxml=unit-report.xml
  artifacts:
    reports:
      junit: unit-report.xml

e2e-tests:
  stage: e2e
  image: mcr.microsoft.com/playwright/python:v1.44.0-jammy
  parallel: 4
  script:
    - pip install -r requirements.txt
    - pytest tests/e2e --shard-id=$CI_NODE_INDEX --num-shards=$CI_NODE_TOTAL
```

## Test sharding и параллелизация

**Test sharding** — разбивка полного набора тестов на N частей, каждая из которых запускается на отдельном CI-воркере. Сокращает общее время прогона линейно: 4 shard = ~4× быстрее.

Нативная поддержка в основных фреймворках:

| Фреймворк | Команда | Без доп. зависимостей |
|---|---|---|
| **Playwright** | `npx playwright test --shard=2/4` | Да |
| **Vitest** | `vitest run --shard=2/4` | Да |
| **Jest** | `jest --shard=2/4` (с v28) | Да |
| **pytest** | `pytest-split` (плагин) | Требует установки |

Дополнительно: **Currents.dev** и **Sorry Cypress** — оркестраторы для Playwright/Cypress, которые распределяют тесты по воркерам динамически (по времени выполнения, а не статически).

## Управление flaky-тестами в CI

Нестабильные тесты (flaky tests) в CI создают ложные провалы и снижают доверие к пайплайну. Паттерн **quarantine** решает это системно: тест помечается как карантинный, не блокирует pipeline, но команда получает уведомление.

### Инструменты для отслеживания flaky-тестов

**BuildPulse** — SaaS, интегрируется с GitHub Actions/CircleCI/Jenkins через upload junit-xml артефактов. Автоматически определяет нестабильные тесты по истории 50+ запусков, создаёт GitHub Issues.

**Currents.dev** — платформа оркестрации для Playwright и Cypress. Dashboard с историей тестов, flakiness score, аналитика по веткам. Поддерживает quarantine mode.

```yaml
# quarantine в GitHub Actions: не блокируем PR из-за нестабильных тестов
- name: Run tests
  run: npx playwright test
  continue-on-error: true

- name: Upload test results to BuildPulse
  uses: buildpulse/buildpulse-action@main
  with:
    account: ${{ secrets.BUILDPULSE_ACCOUNT_ID }}
    repository: ${{ secrets.BUILDPULSE_REPOSITORY_ID }}
    path: test-results/*.xml
    key: ${{ secrets.BUILDPULSE_ACCESS_KEY_ID }}
    secret: ${{ secrets.BUILDPULSE_SECRET_ACCESS_KEY }}
```

## Docker и контейнеризация тестовой среды

Docker решает проблему «у меня работает, а на CI нет»: контейнер гарантирует идентичное окружение на любой машине.

### Playwright в Docker

Playwright предоставляет официальные Docker-образы со всеми браузерами:

```dockerfile
FROM mcr.microsoft.com/playwright:v1.44.0-jammy

WORKDIR /app
COPY package*.json ./
RUN npm ci
COPY . .

CMD ["npx", "playwright", "test"]
```

### Selenoid — сетка браузеров в Docker

**Selenoid** (Aerokube) — лёгкая альтернатива Selenium Grid: запускает каждый тест в отдельном Docker-контейнере с браузером, изолированно.

```yaml
# docker-compose.yml для Selenoid
services:
  selenoid:
    image: aerokube/selenoid:latest
    ports:
      - "4444:4444"
    volumes:
      - /var/run/docker.sock:/var/run/docker.sock
      - ./browsers.json:/etc/selenoid/browsers.json
```

## Testcontainers: реальные зависимости в тестах

**Testcontainers** — библиотека (не платформа), которая запускает настоящие Docker-контейнеры с БД, брокерами сообщений и другими зависимостями прямо во время тестов. Устраняет необходимость мокировать инфраструктуру.

Поддерживаемые языки: Java, Go, Python, Node.js, .NET, Rust.

```typescript
// Node.js + TypeScript
import { PostgreSqlContainer } from '@testcontainers/postgresql';

describe('User repository', () => {
  let container: StartedPostgreSqlContainer;

  beforeAll(async () => {
    container = await new PostgreSqlContainer().start();
  });

  afterAll(async () => {
    await container.stop();
  });

  it('should save and retrieve user', async () => {
    const repo = new UserRepository(container.getConnectionUri());
    await repo.save({ name: 'Alice' });
    const user = await repo.findByName('Alice');
    expect(user).toBeDefined();
  });
});
```

## Cloud execution: фермы устройств и браузеров

Для параллельного E2E на реальных браузерах и устройствах используются облачные платформы.

| Платформа | Особенность | Когда выбирать |
|---|---|---|
| **BrowserStack** | 20 000+ реальных устройств; Percy visual testing | Cross-browser, мобильное; широкий охват |
| **LambdaTest** | Лучшее соотношение цена/качество; KaneAI | Стартапы и растущие команды |
| **Sauce Labs** | SOC2/ISO 27001; enterprise compliance | Регулируемые отрасли (fintech, healthcare) |
| **AWS Device Farm** | AWS-native; интеграция с CodePipeline | AWS-инфраструктура |
| **Firebase Test Lab** | Реальные Android-устройства; бесплатный tier | Android / Google Play |

## Отчётность

Стандарт передачи результатов в CI — **JUnit XML** формат. Почти все фреймворки умеют его генерировать.

**Allure Report** — популярный инструмент для HTML-отчётов: история тестов, категории провалов, шаги со скриншотами.

**Playwright HTML Report** — встроенный, без зависимостей. Включает трассы, видео, скриншоты для каждого упавшего теста: `npx playwright show-report`.

## Источники

* [GitHub Actions documentation](https://docs.github.com/en/actions)
* [GitLab CI/CD documentation](https://docs.gitlab.com/ee/ci/)
* [Playwright: CI/CD guide](https://playwright.dev/docs/ci)
* [Testcontainers documentation](https://testcontainers.com/guides/)
* [Selenoid documentation](https://aerokube.com/selenoid/latest/)
* [BuildPulse — flaky test management](https://buildpulse.io)
* [Currents.dev — Playwright orchestration](https://currents.dev)
* [Allure Framework](https://allurereport.org)
* [Martin Fowler: Continuous Integration](https://martinfowler.com/articles/continuousIntegration.html)

### Дополнительные материалы

* [Идеальный пайплайн в вакууме](https://habr.com/ru/company/rabota/blog/560922/) — практические примеры stages в реальных проектах
* [Создаем инфраструктуру для интеграционных тестов](https://habr.com/ru/company/2gis/blog/575688/) — кейс от 2GIS с Docker и CI
* [DevOps инструменты не только для DevOps](https://habr.com/ru/post/497918/) — построение инфраструктуры автоматизации с нуля
* [Зачем CI/CD тестировщикам?](https://habr.com/ru/company/JetBrains/blog/650757/) — обзор от JetBrains
