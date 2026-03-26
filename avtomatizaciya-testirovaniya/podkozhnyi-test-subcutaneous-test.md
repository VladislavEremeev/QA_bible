# Подкожный тест (Subcutaneous Test)

UI-тесты — самый дорогой уровень автоматизации: медленные, нестабильные, сложные в написании и поддержке. При этом значительная часть бизнес-логики не требует браузера для проверки. Подкожный тест — альтернатива: тест непосредственно под слоем пользовательского интерфейса, проверяющий реальную логику без накладных расходов на браузер.

## Определение

**Подкожный тест (Subcutaneous Test)** — автоматизированный тест, работающий непосредственно под слоем UI: для MVC-приложений — всё под контроллером, для веб-сервисов — под endpoint'ом.

Термин впервые использовал Jimmy Bogard (2010): «В то время как unit-тест фокусируется на мелкомасштабном дизайне, подкожный тест проверяет основные входы и выходы системы в целом».

## Почему не UI-тесты

* UI-тесты медленные — браузер всегда добавляет задержки
* UI-тесты нестабильные — частично из-за скорости, частично из-за того что браузер не создан для программного управления
* UI-тесты тестируют слишком много сразу — сложно локализовать причину падения
* UI-тесты симулируют пользователя неточно — пользователь не ищет элемент по XPath и не кликает со скоростью программы

Если функционал нельзя протестировать иначе как через UI — это может быть признаком архитектурных проблем.

## Как работают подкожные тесты

Тест вызывает сервисный слой или Use Case напрямую, минуя UI. HTTP-запросы к реальным сервисам могут быть замоканы через MSW или WireMock. Результат — быстрые, стабильные тесты, проверяющие полный бизнес-сценарий без браузера.

В React-приложениях это Testing Library: тест рендерит компонент в jsdom, взаимодействует с ним как пользователь (по тексту, роли, label), но без настоящего браузера.

## Современные инструменты

### Vitest

**Vitest** — быстрый test runner для JavaScript/TypeScript, совместимый с Jest API. Использует Vite для трансформации кода, что даёт существенное ускорение на современных проектах. Поддерживает ESM нативно, параллельное выполнение, coverage через v8.

```typescript
import { describe, it, expect } from 'vitest';
import { UserService } from './UserService';

describe('UserService', () => {
  it('should create user with hashed password', async () => {
    const service = new UserService(mockDb);
    const user = await service.create({ name: 'Alice', password: 'secret' });
    expect(user.password).not.toBe('secret');
    expect(user.name).toBe('Alice');
  });
});
```

### Testing Library

**Testing Library** (`@testing-library/react`, `/vue`, `/angular`) — стандарт для компонентного тестирования. Философия: тестировать компоненты так, как ими пользуется пользователь — по тексту, роли, label, а не по CSS-классам или internal state.

```typescript
import { render, screen, userEvent } from '@testing-library/react';
import { LoginForm } from './LoginForm';

test('submits form with credentials', async () => {
  const onSubmit = vi.fn();
  render(<LoginForm onSubmit={onSubmit} />);

  await userEvent.type(screen.getByLabelText('Email'), 'user@example.com');
  await userEvent.type(screen.getByLabelText('Password'), 'secret');
  await userEvent.click(screen.getByRole('button', { name: 'Log in' }));

  expect(onSubmit).toHaveBeenCalledWith({ email: 'user@example.com', password: 'secret' });
});
```

### MSW (Mock Service Worker)

**MSW** — мокирование API на уровне сети через Service Worker (в браузере) или Node.js interceptor (в тестах). Тест получает реалистичное API-взаимодействие без реального сервера.

```typescript
import { http, HttpResponse } from 'msw';
import { setupServer } from 'msw/node';

const server = setupServer(
  http.get('/api/users/:id', ({ params }) => {
    return HttpResponse.json({ id: params.id, name: 'Alice' });
  })
);

beforeAll(() => server.listen());
afterEach(() => server.resetHandlers());
afterAll(() => server.close());
```

## Соотношение с другими видами тестов

Подкожные тесты не заменяют UI-тесты полностью — они уменьшают их необходимое количество. UI-тесты в этой схеме становятся smoke-тестами: «приложение запустилось и все слои связаны». Основная бизнес-логика проверяется подкожно или unit-тестами.

Снижение покрытия glue code (связующего кода между слоями) — допустимый компромисс, если этот код прост и редко меняется.

## Источники

* [Introduction To Subcutaneous Testing](https://www.ministryoftesting.com/dojo/lessons/introduction-to-subcutaneous-testing)
* [Martin Fowler: SubcutaneousTest](https://martinfowler.com/bliki/SubcutaneousTest.html)
* [Пишем автотесты эффективно — Subcutaneous tests](https://habr.com/ru/post/502154/)
* [Vitest — документация](https://vitest.dev)
* [Testing Library — документация](https://testing-library.com)
* [MSW — Mock Service Worker](https://mswjs.io)

### Дополнительные материалы

* [Microtesting — How We Set Fire To The Testing Pyramid](https://www.youtube.com/watch?v=pls1Vk_bw_Y) — доклад NDC о подкожном тестировании
* [Subcutaneous Testing in ASP.NET Core](https://josephwoodward.co.uk/2019/03/subcutaneous-testing-asp-net-core) — пример для .NET
