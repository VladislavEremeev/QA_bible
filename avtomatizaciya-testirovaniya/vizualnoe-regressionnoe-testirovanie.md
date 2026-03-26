# Визуальное регрессионное тестирование (Visual Regression Testing)

Функциональные тесты проверяют поведение, но не замечают визуальные баги: сдвинутые элементы, неправильные цвета, обрезанный текст, сломанную вёрстку в конкретном браузере. Визуальное регрессионное тестирование автоматизирует сравнение скриншотов UI между базовым состоянием и текущим, выявляя непреднамеренные изменения внешнего вида.

## Определение

**Визуальное регрессионное тестирование (Visual Regression Testing)** — автоматическое сравнение скриншотов или рендеров компонентов с эталонными изображениями (baseline) для обнаружения непреднамеренных визуальных изменений.

Baseline создаётся при первом запуске или вручную. При последующих запусках инструмент делает новый скриншот, вычисляет разницу (diff) и либо сообщает о допустимом отклонении, либо помечает тест как упавший.

## Инструменты

### Playwright встроенные скриншоты

Playwright предоставляет визуальное тестирование из коробки — без дополнительных библиотек.

```typescript
import { test, expect } from '@playwright/test';

test('homepage visual test', async ({ page }) => {
  await page.goto('https://example.com');
  // Сравнить с baseline screenshot
  await expect(page).toHaveScreenshot('homepage.png');
});

test('button component', async ({ page }) => {
  const button = page.locator('.submit-btn');
  // Скриншот конкретного элемента
  await expect(button).toHaveScreenshot('submit-button.png', {
    threshold: 0.1,  // допустимое отклонение 10%
  });
});
```

Baseline хранится в репозитории рядом с тестами (`.spec.ts-snapshots/`). При изменении baseline: `npx playwright test --update-snapshots`.

Особенности:
* Pixel-by-pixel сравнение с настраиваемым threshold
* Cross-browser из коробки (Chromium, Firefox, WebKit)
* Нет внешних зависимостей и SaaS
* Подходит для небольших проектов или точечных проверок

{% hint style="warning" %}
Pixel-by-pixel сравнение чувствительно к субпиксельным рендеринг-различиям между браузерами и ОС. На разных машинах baseline может отличаться — используй Docker для стабильного окружения.
{% endhint %}

### Percy (BrowserStack)

**Percy** — облачная платформа визуального тестирования от BrowserStack. Интегрируется через SDK в существующие тесты. Главная особенность — кросс-браузерные снимки и AI Visual Review Agent.

```bash
npm install --save-dev @percy/cli @percy/playwright
```

```typescript
import { percySnapshot } from '@percy/playwright';

test('checkout page visual test', async ({ page }) => {
  await page.goto('/checkout');
  await percySnapshot(page, 'Checkout Page');
  // Percy делает снимок и отправляет в облако
});
```

```bash
# Запуск с Percy
PERCY_TOKEN=<token> percy exec -- npx playwright test
```

Особенности:
* **AI Visual Review Agent** — фильтрует ~40% ложных срабатываний (шрифт-рендеринг, subpixel-различия)
* Автоматически делает снимки в Chrome, Firefox, Safari на нескольких viewport
* PR-интеграция: Percy добавляет visual diff прямо в GitHub/GitLab PR
* SDK доступен для Playwright, Cypress, Selenium, WebdriverIO, Storybook

### Chromatic

**Chromatic** — платформа визуального тестирования на уровне компонентов, тесно интегрированная со Storybook. Оптимальна для design systems и библиотек компонентов.

```bash
npm install --save-dev chromatic
npx chromatic --project-token=<token>
```

Особенности:
* **TurboSnap** — анализирует git diff и делает снимки только изменённых компонентов (ускоряет в 5–10×)
* Каждый Story в Storybook автоматически становится визуальным тестом
* Перехватывает изменения на уровне компонента, не страницы
* Интеграция с GitHub, GitLab, Bitbucket: статус-чек в PR
* UI Review workflow: дизайнеры и разработчики принимают/отклоняют визуальные изменения

### Applitools Eyes

**Applitools Eyes** — enterprise-класс визуального тестирования с Visual AI (нейросеть, обученная на 1B+ изображений).

```typescript
import { Eyes, Target } from '@applitools/eyes-playwright';

test('product page visual test', async ({ page }) => {
  const eyes = new Eyes();
  await eyes.open(page, 'My App', 'Product Page Test');
  await page.goto('/product/123');
  await eyes.check('Product Page', Target.window().fully());
  await eyes.close();
});
```

Особенности:
* **Visual AI** понимает контент, не пиксели — отличает значимые изменения от шума рендеринга
* **Ultrafast Test Cloud** — параллельный кросс-браузерный захват без замедления тестов
* SDK для всех major фреймворков: Playwright, Cypress, Selenium, WebdriverIO, Appium
* Интеграция с Jira, Slack, Teams для управления визуальными багами
* Подходит для сложных dynamic-контентных страниц

## Сравнительная таблица

| Критерий | Playwright built-in | Percy | Chromatic | Applitools |
|---|---|---|---|---|
| Уровень тестирования | Страница / компонент | Страница | Компонент (Storybook) | Страница / компонент |
| Cross-browser | Да (3 браузера) | Да (AI-рендеринг) | Ограничено | Да (Ultrafast Cloud) |
| AI-фильтрация шума | Нет | Да (~40% экономия) | Нет | Да (Visual AI) |
| Хранение baseline | В репозитории | SaaS | SaaS | SaaS |
| Бесплатный tier | Полностью бесплатно | Ограниченно | Ограниченно | Trial |
| Storybook-интеграция | Нет | Частично | Нативно | Да |
| Open source | Да | Нет | Нет | Нет |

## Когда что выбирать

* **Минимальная настройка, baseline в Git** — Playwright built-in; использовать Docker для стабильного рендеринга
* **Кросс-браузерная регрессия страниц в CI** — Percy; особенно если уже используется BrowserStack
* **Design system / компонентная библиотека со Storybook** — Chromatic; TurboSnap делает его быстрым
* **Enterprise, динамический контент, нужна Visual AI** — Applitools Eyes

## Источники

* [Playwright: Visual comparisons](https://playwright.dev/docs/test-snapshots)
* [Percy documentation](https://docs.percy.io)
* [Chromatic documentation](https://www.chromatic.com/docs/)
* [Applitools Eyes documentation](https://applitools.com/docs/)
* [Awesome Visual Regression Testing](https://github.com/mojoaxel/awesome-regression-testing)

### Дополнительные материалы

* [Александр Самойлов — Визуальные проверки в End-to-End тестах](https://www.youtube.com/watch?v=RSNZ2312XJI) — доклад о практическом применении
* [Внедряем Snapshot testing в UI-тесты iOS](https://habr.com/ru/company/vivid_money/blog/569032/) — аналогичный подход для нативных приложений
