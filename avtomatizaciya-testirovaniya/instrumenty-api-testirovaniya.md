# Инструменты API-тестирования (API Testing Tools)

API-тестирование проверяет бизнес-логику и контракты сервисов независимо от пользовательского интерфейса. Тесты на уровне API быстрее E2E в 10–100 раз, стабильнее (нет проблем с DOM и браузерными задержками) и дают более точную диагностику при падении. Зрелая стратегия тестирования предполагает основную часть автоматизации именно на этом уровне.

## Инструменты

### Bruno

**Bruno** — open-source десктопный клиент для работы с API, появившийся как прямая альтернатива Postman после изменений в его ценовой политике (2023). Ключевое отличие: коллекции хранятся как plain-text файлы в файловой системе, что делает их пригодными для хранения в Git наравне с остальным кодом.

Особенности:
* Коллекции — директории с `.bru` файлами (plaintext формат), не JSON/BSON
* Нет облачной синхронизации — всё локально или в Git
* CLI (`@usebruno/cli`) для запуска в CI: `bru run --env production`
* Поддержка: REST, GraphQL, WebSocket
* Скриптинг на JavaScript для pre-request и post-response

```bash
# Запуск коллекции в CI
npx @usebruno/cli run collection/ --env staging --reporter junit
```

### Playwright API Testing

**Playwright** включает встроенный HTTP-клиент для API-тестирования — без дополнительных зависимостей. Позволяет комбинировать API и UI в одном тесте: например, создать тестовые данные через API, проверить их отображение через UI.

```typescript
import { test, expect } from '@playwright/test';

test('create and verify user via API', async ({ request }) => {
  // Создать пользователя
  const response = await request.post('/api/users', {
    data: { name: 'Alice', email: 'alice@example.com' }
  });
  expect(response).toBeOK();

  const user = await response.json();
  expect(user.name).toBe('Alice');

  // Проверить что пользователь доступен
  const getResponse = await request.get(`/api/users/${user.id}`);
  expect(getResponse).toBeOK();
});
```

Особенности:
* Нет отдельной установки — входит в Playwright
* Та же система fixtures, `beforeAll`/`afterAll`
* `APIRequestContext` можно использовать в setup-файлах для подготовки данных
* Поддержка HAR-записи для отладки

### REST Assured

**REST Assured** — Java-библиотека для тестирования REST API в BDD-стиле (`given().when().then()`). Стандарт для Java-команд, работает в связке с JUnit 5 и TestNG.

```java
import static io.restassured.RestAssured.*;
import static org.hamcrest.Matchers.*;

@Test
void shouldReturnUserById() {
    given()
        .baseUri("https://api.example.com")
        .header("Authorization", "Bearer " + token)
    .when()
        .get("/users/1")
    .then()
        .statusCode(200)
        .body("name", equalTo("Alice"))
        .body("email", notNullValue());
}
```

Особенности:
* Первоклассная интеграция с Spring Boot (`RestAssuredMockMvc`)
* Поддержка JSON Schema validation
* OAuth 2.0, Basic Auth, certificate auth из коробки
* JSON и XML body matching через Hamcrest и JsonPath

### Postman / Newman

**Postman** — наиболее известный API-клиент. Несмотря на изменения в pricing (2023), остаётся популярным. **Newman** — CLI для запуска Postman-коллекций в CI.

```bash
newman run collection.json -e environment.json --reporters cli,junit --reporter-junit-export results.xml
```

{% hint style="warning" %}
Postman перевёл локальное хранение коллекций в платный план (Scratch Pad ограничен). Команды, ищущие бесплатную альтернативу с Git-интеграцией, переходят на Bruno или Hoppscotch.
{% endhint %}

### Hoppscotch

**Hoppscotch** — web-based open-source клиент. Работает в браузере без установки, поддерживает REST, GraphQL, WebSocket, gRPC, Server-Sent Events. Есть self-hosted вариант.

* Быстрый старт — открыть hoppscotch.io и работать
* Коллекции синхронизируются через аккаунт
* GraphQL-поддержка с introspection и автодополнением
* CLI для CI: `@hoppscotch/cli`

## Сравнительная таблица

| Критерий | Bruno | Playwright API | REST Assured | Postman | Hoppscotch |
|---|---|---|---|---|---|
| Язык/формат тестов | JavaScript | TypeScript/JS | Java | JavaScript | JavaScript |
| Git-friendly | Да (plain text) | Да (код) | Да (код) | Нет (JSON) | Частично |
| CI-интеграция | Bruno CLI | npx playwright | JUnit/Maven | Newman CLI | Hoppscotch CLI |
| GraphQL | Да | Нет | Нет | Да | Да |
| Бесплатно | Да (open-source) | Да (open-source) | Да (open-source) | Ограничено | Да (open-source) |
| Комбинация API+UI | Нет | Да | Нет | Нет | Нет |
| Целевая аудитория | Разработчики/QA | QA (Playwright-стек) | Java-команды | Все | Все |

## Когда что выбирать

* **Новый проект на TypeScript + Playwright** — используй встроенный API testing, не вводи отдельный инструмент
* **Java-стек (Spring Boot)** — REST Assured как стандарт
* **Нужны коллекции в Git + нет Postman-бюджета** — Bruno
* **Быстрая проверка API без установки** — Hoppscotch в браузере
* **Унаследованные Postman-коллекции** — Newman в CI, постепенная миграция на Bruno

## Источники

* [Bruno documentation](https://docs.usebruno.com)
* [Playwright API testing guide](https://playwright.dev/docs/api-testing)
* [REST Assured documentation](https://rest-assured.io)
* [Hoppscotch](https://hoppscotch.io)
* [Newman — Postman CLI](https://learning.postman.com/docs/collections/using-newman-cli/command-line-integration-with-newman/)

### Дополнительные материалы

* [Тестирование API с помощью REST Assured](https://medium.com/@svetlana.podv/тестирование-api-с-помощью-rest-assured-2654f9b1faab) — практический туториал на Java
* [Playwright API Testing vs REST Assured](https://playwright.dev/docs/api-testing) — сравнение подходов
