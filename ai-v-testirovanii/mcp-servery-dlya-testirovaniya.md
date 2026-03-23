# MCP серверы для тестирования (Model Context Protocol)

**Model Context Protocol (MCP)** — открытый протокол, разработанный Anthropic в 2024 году, который стандартизирует способ подключения AI-агентов к внешним инструментам, данным и сервисам. MCP позволяет AI-модели не просто генерировать текст, а взаимодействовать с браузером, базой данных, файловой системой, CI/CD-пайплайном — всем, что нужно для реального тестирования.

Если AI-агент — это голова, то MCP-серверы — это руки. Без них агент может только рассуждать; с ними — действовать.

---

## Архитектура MCP

MCP работает по модели клиент-сервер:

```
AI-агент (Claude Code, Cursor, Claude Desktop)
         │
    MCP Client
         │  (JSON-RPC over stdio / HTTP)
         │
    MCP Server
         │
   Внешний сервис
   (браузер, БД, API, файловая система)
```

**MCP Host** — приложение, в котором работает AI (Claude Code, Claude Desktop, Cursor).
**MCP Client** — встроенный в host компонент, управляющий соединениями с серверами.
**MCP Server** — отдельный процесс, предоставляющий инструменты и ресурсы.

### Три типа сущностей в MCP

| Тип | Описание | Пример |
|-----|----------|--------|
| **Tools** | Функции, которые агент может вызвать | `browser_click`, `run_sql`, `get_pr_status` |
| **Resources** | Данные, которые агент может прочитать | Файл логов, снимок БД, OpenAPI-спецификация |
| **Prompts** | Готовые шаблоны для типовых задач | "Проверь этот PR на безопасность" |

---

## Как MCP применяется в тестировании

### 1. Браузерное тестирование

MCP-серверы для браузера дают агенту возможность управлять браузером так же, как это делает Selenium или Playwright — но через естественный язык:

**Playwright MCP** (`@playwright/mcp`) — официальный MCP-сервер от Microsoft:
- Открытие URL, клики, заполнение форм
- Скриншоты и снимки DOM
- Перехват сетевых запросов
- Запуск тестов и получение результатов

```
Агент получает задачу: "Проверь форму регистрации"

Агент → MCP Playwright → browser_navigate("https://app.example.com/register")
Агент → MCP Playwright → browser_screenshot()
Агент анализирует снимок, определяет поля
Агент → MCP Playwright → browser_fill("#email", "test@example.com")
Агент → MCP Playwright → browser_click("#submit")
Агент → MCP Playwright → browser_screenshot()
Агент сравнивает результат с ожидаемым поведением
```

**Puppeteer MCP** — аналог для Chrome DevTools Protocol.

### 2. Тестирование баз данных

MCP-серверы для БД позволяют агенту проверять состояние данных напрямую:

```
Агент после создания пользователя через UI:
→ MCP PostgreSQL → query("SELECT * FROM users WHERE email = 'test@example.com'")
→ Проверяет, что запись создана, поля заполнены корректно, хеш пароля не пустой
```

Доступные серверы:
- `@modelcontextprotocol/server-postgres` — PostgreSQL
- `@modelcontextprotocol/server-sqlite` — SQLite
- Серверы для MySQL, MongoDB, Redis

### 3. Тестирование API

MCP-серверы для HTTP-запросов:

```
Агент → MCP HTTP → POST /api/users {name: "Test", email: "t@t.com"}
Агент → Проверяет статус 201, структуру ответа, заголовки
Агент → MCP PostgreSQL → Проверяет запись в БД
Агент → MCP HTTP → GET /api/users/{id}
Агент → Сравнивает данные в ответе с данными в БД
```

### 4. Интеграция с системами управления тестами

- **Jira MCP** — создание баг-репортов, обновление задач, получение требований
- **GitHub MCP** (`@modelcontextprotocol/server-github`) — работа с PR, issues, CI-статусами
- **Linear MCP** — управление задачами в Linear

### 5. Файловая система и артефакты

`@modelcontextprotocol/server-filesystem` — доступ к локальным файлам:
- Чтение тест-кейсов из файлов
- Сохранение отчётов о тестировании
- Анализ логов приложения

---

## Установка и конфигурация

MCP-серверы конфигурируются в файлах настроек AI-клиента.

### Для Claude Code (`~/.claude/claude.json`):

```json
{
  "mcpServers": {
    "playwright": {
      "command": "npx",
      "args": ["@playwright/mcp@latest"]
    },
    "postgres": {
      "command": "npx",
      "args": ["-y", "@modelcontextprotocol/server-postgres"],
      "env": {
        "DATABASE_URL": "postgresql://user:pass@localhost/testdb"
      }
    },
    "github": {
      "command": "npx",
      "args": ["-y", "@modelcontextprotocol/server-github"],
      "env": {
        "GITHUB_TOKEN": "ghp_xxxx"
      }
    }
  }
}
```

### Для Claude Desktop (`claude_desktop_config.json`):

```json
{
  "mcpServers": {
    "playwright": {
      "command": "npx",
      "args": ["@playwright/mcp@latest", "--headless"]
    }
  }
}
```

---

## Создание собственного MCP-сервера для тестирования

Если стандартных серверов недостаточно, можно написать свой. MCP SDK доступен для TypeScript и Python.

### Пример: MCP-сервер для тестовой среды

```python
from mcp.server import Server
from mcp.server.stdio import stdio_server
from mcp.types import Tool, TextContent
import httpx

app = Server("test-environment-mcp")

@app.list_tools()
async def list_tools():
    return [
        Tool(
            name="reset_test_db",
            description="Сбрасывает тестовую БД к начальному состоянию",
            inputSchema={"type": "object", "properties": {}}
        ),
        Tool(
            name="seed_test_data",
            description="Заполняет БД тестовыми данными",
            inputSchema={
                "type": "object",
                "properties": {
                    "scenario": {
                        "type": "string",
                        "description": "Название сценария: basic, premium, admin"
                    }
                }
            }
        ),
        Tool(
            name="get_app_logs",
            description="Получает последние логи приложения",
            inputSchema={
                "type": "object",
                "properties": {
                    "lines": {"type": "number", "description": "Количество строк"}
                }
            }
        )
    ]

@app.call_tool()
async def call_tool(name: str, arguments: dict):
    if name == "reset_test_db":
        # Вызов endpoint тестового окружения
        async with httpx.AsyncClient() as client:
            await client.post("http://test-env/reset")
        return [TextContent(type="text", text="БД сброшена")]

    elif name == "seed_test_data":
        scenario = arguments.get("scenario", "basic")
        async with httpx.AsyncClient() as client:
            await client.post(f"http://test-env/seed/{scenario}")
        return [TextContent(type="text", text=f"Данные сценария '{scenario}' загружены")]

if __name__ == "__main__":
    import asyncio
    asyncio.run(stdio_server(app))
```

### Типовые инструменты для QA MCP-сервера

```
test_environment_mcp/
├── tools/
│   ├── reset_db          — сброс тестовой БД
│   ├── seed_data         — загрузка фикстур
│   ├── get_logs          — получение логов приложения
│   ├── clear_cache       — очистка кешей
│   ├── mock_service      — включение/выключение мок-сервисов
│   └── get_feature_flags — получение актуальных фичер-флагов
└── resources/
    ├── test_cases        — тест-кейсы из тестовой документации
    ├── api_spec          — OpenAPI-спецификация
    └── known_bugs        — список известных багов
```

---

## Популярные MCP-серверы для QA

| Сервер | Назначение | Установка |
|--------|------------|-----------|
| `@playwright/mcp` | E2E-тестирование браузера | `npx @playwright/mcp` |
| `@modelcontextprotocol/server-postgres` | Проверка данных в PostgreSQL | `npx @modelcontextprotocol/server-postgres` |
| `@modelcontextprotocol/server-github` | Работа с PR, issues, CI | `npx @modelcontextprotocol/server-github` |
| `@modelcontextprotocol/server-filesystem` | Работа с файлами и логами | `npx @modelcontextprotocol/server-filesystem` |
| `@modelcontextprotocol/server-fetch` | HTTP-запросы к API | `npx @modelcontextprotocol/server-fetch` |
| `mcp-server-jira` | Создание баг-репортов в Jira | `npx mcp-server-jira` |
| `mcp-server-slack` | Уведомления о результатах | `npx mcp-server-slack` |

Актуальный каталог серверов: [github.com/modelcontextprotocol/servers](https://github.com/modelcontextprotocol/servers)

---

## Паттерны использования MCP в QA-процессах

### Паттерн 1: Автономное исследовательское тестирование

```
Агент получает: "Протестируй процесс оформления заказа"

1. [Playwright MCP] Открывает магазин, делает скриншот
2. Анализирует UI, строит план тестирования
3. [Playwright MCP] Проходит по каждому шагу оформления
4. [PostgreSQL MCP] Проверяет создание заказа в БД
5. [HTTP MCP] Проверяет вызов payment API
6. Формирует отчёт о найденных проблемах
7. [GitHub MCP] Создаёт issue на каждый дефект
```

### Паттерн 2: Регрессионное тестирование по изменениям в PR

```
Триггер: новый PR в GitHub

1. [GitHub MCP] Читает список изменённых файлов
2. Определяет затронутые функции/компоненты
3. [Filesystem MCP] Читает существующие тест-кейсы
4. [Playwright MCP] Запускает релевантные E2E-тесты
5. [PostgreSQL MCP] Проверяет целостность данных
6. [GitHub MCP] Постит результаты как комментарий к PR
```

### Паттерн 3: Тест-оракул через MCP

```
Агент сравнивает поведение:
[HTTP MCP] → production endpoint  → response_prod
[HTTP MCP] → staging endpoint     → response_staging
Сравнивает структуру, данные, время ответа
Выявляет расхождения, создаёт отчёт
```

---

## Ограничения и риски

**Безопасность:**
- MCP-серверы имеют доступ к реальным системам — необходима изоляция (тестовые среды, не продакшн)
- Токены и credentials должны передаваться через переменные окружения, не в конфиге
- Стоит ограничивать права доступа (read-only для большинства инструментов)

**Надёжность:**
- Если MCP-сервер упал, агент теряет доступ к инструменту
- Нужен мониторинг доступности серверов

**Детерминизм:**
- Агент может выбирать разные инструменты в разных запусках
- Для регрессионных тестов важна воспроизводимость сценариев

---

## Связанные материалы

- [Agentic Development](agentic-development.md)
- [Claude Code](claude-code.md)
- [AI-Driven Development](ai-driven-development.md)
- [Context Engineering](context-engineering.md)
