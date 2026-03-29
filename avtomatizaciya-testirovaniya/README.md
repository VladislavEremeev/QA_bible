# Автоматизация тестирования (Automation Testing)

Автоматизация тестирования — использование программных инструментов для выполнения тестов без ручного вмешательства. В отличие от ручного тестирования, автоматизированные тесты запускаются в CI/CD-пайплайне при каждом изменении кода, обеспечивая быструю обратную связь команде. Этот раздел охватывает теорию, актуальный инструментарий и практики автоматизации для QA-специалистов.

## Содержание раздела

### Основы

* [Общее](obshee.md) — что такое автоматизация, зачем нужна, когда применять
* [Что автоматизировать](chto-nuzhno-avtomatizirovat.md) — критерии выбора
* [Лучшие практики](luchshie-praktiki-avtomatizacii.md) — принципы и антипаттерны

### Инструменты и фреймворки

* [Виды и инструменты автоматизации](vidy-i-instrumenty-avtomatizacii.md) — обзор фреймворков: Playwright, Cypress, Selenium, Appium, Maestro, k6
* [Инструменты API-тестирования](instrumenty-api-testirovaniya.md) — Bruno, Playwright API, REST Assured, Hoppscotch
* [Визуальное регрессионное тестирование](vizualnoe-regressionnoe-testirovanie.md) — Percy, Chromatic, Applitools, Playwright screenshots

### CI/CD и инфраструктура

* [Инфраструктура и пайплайн (CI/CD)](infrastruktura-i-paiplain-ci-cd.md) — GitHub Actions, GitLab CI, Docker, Testcontainers
* [Процессы и автоматизация с нуля](processy-i-avtomatizaciya-proekta-s-nulya.md) — кейс построения автоматизации

### Техники и паттерны

* [Параллельное тестирование](parallelnoe-testirovanie-parallel-testing.md) — sharding, cloud execution, изоляция
* [Flaky tests](chto-takoe-flaky-tests.md) — причины, диагностика, инструменты карантина
* [Мутационное тестирование](mutacionnoe-testirovanie-mutation-testing.md) — Stryker, PIT, mutmut
* [Подкожный тест](podkozhnyi-test-subcutaneous-test.md) — subcutaneous подход, Testing Library
* [Coupling и Cohesion](raznica-mezhdu-coupling-i-cohesion.md) — влияние на тестируемость кода

### Карьера

* [Как стать автоматизатором](kak-stat-avtomatizatorom-i-voprosy-s-sobesedovanii.md) — пути развития и вопросы с собеседований

### Ресурсы

* [Полезные ссылки](poleznye-ssylki.md) — документация, курсы, сообщества
