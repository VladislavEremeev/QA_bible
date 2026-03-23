# AI агентные инструменты: Claude Code, Gemini CLI, Qwen Code и другие

Агентные AI-инструменты — это CLI и IDE-расширения, дающие языковым моделям доступ к реальной кодовой базе: чтение и редактирование файлов, выполнение команд, работа с git, запуск тестов. В отличие от чат-интерфейсов, они **действуют в вашем проекте**, а не просто отвечают на вопросы.

В 2024–2026 годах сложилась конкурентная экосистема таких инструментов от разных вендоров. Эта статья охватывает основные инструменты, их возможности и способы расширения для задач QA.

---

## Обзор инструментов

| Инструмент | Вендор | Модель | Тип | Открытый код |
|------------|--------|--------|-----|--------------|
| Claude Code | Anthropic | Claude Sonnet/Opus | CLI-агент | Нет |
| Gemini CLI | Google | Gemini 2.5 Pro | CLI-агент | Да |
| Qwen Code | Alibaba | Qwen2.5-Coder | CLI-агент | Да |
| Aider | Community | Любая LLM | CLI-агент | Да |
| OpenHands | Community | Любая LLM | Web + CLI | Да |
| Cursor Agent | Anysphere | Claude / GPT-4 | IDE (VS Code fork) | Нет |
| GitHub Copilot Agent | Microsoft | GPT-4o | IDE + CLI | Нет |

---

## Claude Code

**Anthropic** | [docs.anthropic.com/claude-code](https://docs.anthropic.com/claude-code)

Флагман линейки. Работает в терминале, имеет прямой доступ к файловой системе, bash, git. Поддерживает MCP-серверы для расширения возможностей.

```bash
npm install -g @anthropic-ai/claude-code
claude
```

**Сильные стороны для QA:**
- Параллельные субагенты для тестирования нескольких модулей
- Hooks для автоматизации (запуск линтера после правки, логирование)
- Глубокая интеграция с MCP (Playwright, Postgres, GitHub)
- CLAUDE.md для настройки контекста проекта

**Ограничения:**
- Платный (требует API-ключ или подписку Pro/Max)
- Закрытый исходный код

Подробнее: [Claude Code](claude-code.md)

---

## Gemini CLI

**Google** | [github.com/google-gemini/gemini-cli](https://github.com/google-gemini/gemini-cli)

Открытый CLI-агент от Google на базе модели Gemini 2.5 Pro. Запускается в терминале, работает с файлами и командами. Особенность — **бесплатный tier** через Google AI Studio (до 60 запросов/минуту, 1000 запросов/день на момент выхода).

```bash
npm install -g @google/gemini-cli
gemini
```

### Возможности

- Работа с файловой системой (чтение, запись, редактирование)
- Выполнение shell-команд
- Поиск по файлам (glob, grep)
- Браузерное взаимодействие через встроенный инструмент
- Поддержка MCP-серверов (совместим со стандартом)

### Gemini CLI для QA

```
# Анализ тестового покрытия
> Посмотри на тесты в tests/ и код в src/ — какие функции не покрыты тестами?

# Поиск потенциальных багов
> Найди все места, где входные данные от пользователя не валидируются

# Генерация тест-данных
> Создай 50 тестовых пользователей с разными комбинациями прав доступа для нагрузочного теста
```

### Расширение Gemini CLI

**MCP-серверы** — Gemini CLI совместим со стандартом MCP:

```json
// .gemini/settings.json
{
  "mcpServers": {
    "playwright": {
      "command": "npx",
      "args": ["@playwright/mcp@latest"]
    }
  }
}
```

**Собственные инструменты** — через расширение `tools`:

```javascript
// gemini-tools/run-tests.js
export const runTests = {
  name: "run_tests",
  description: "Запускает тесты и возвращает результат",
  parameters: {
    type: "object",
    properties: {
      pattern: { type: "string", description: "Паттерн файлов тестов" }
    }
  },
  execute: async ({ pattern }) => {
    const { execSync } = require("child_process");
    return execSync(`pytest ${pattern} -v`).toString();
  }
};
```

**GEMINI.md** — файл контекста проекта (аналог CLAUDE.md):

```markdown
# GEMINI.md

## Проект
E2E тестирование платёжного сервиса

## Запуск тестов
- Все тесты: `pytest tests/ -v`
- Только smoke: `pytest tests/ -m smoke`
- Coverage: `pytest --cov=src --cov-report=html`

## Тестовые данные
Фикстуры: `tests/fixtures/`
Фабрики: `tests/factories.py`
```

---

## Qwen Code

**Alibaba Cloud** | [github.com/QwenLM/qwen-code](https://github.com/QwenLM/qwen-code)

Открытый CLI-агент на базе модели Qwen2.5-Coder. Fork проекта Gemini CLI, адаптированный под модели Qwen. Полностью совместим с локальными моделями через Ollama или vLLM — возможность запустить агента **без отправки данных в облако**.

```bash
npm install -g qwen-code
qwen
```

### Особенности

**Локальный запуск через Ollama:**

```bash
# Установка модели
ollama pull qwen2.5-coder:32b

# Запуск Qwen Code с локальной моделью
QWEN_API_BASE=http://localhost:11434 qwen
```

Это критически важно для проектов с NDA, закрытым исходным кодом, банковским или государственным ПО — данные не покидают инфраструктуру.

**Конфигурация для корпоративной среды:**

```json
// ~/.qwen/settings.json
{
  "model": "qwen2.5-coder:32b",
  "apiBase": "http://internal-llm-server.company.com/v1",
  "apiKey": "internal-key"
}
```

### Qwen Code для QA

```
# Аудит безопасности (локально, без утечки кода)
> Проверь auth/ на наличие уязвимостей OWASP Top 10

# Анализ legacy-кода
> Объясни, что делает этот модуль и напиши тесты для него
```

---

## Aider

**Community** | [aider.chat](https://aider.chat)

Ветеран среди CLI-агентов (2023). Поддерживает любую LLM через OpenAI-совместимый API. Специализируется на изменениях в коде через git — каждое изменение автоматически коммитится.

```bash
pip install aider-chat
aider --model claude-3-7-sonnet-20250219
```

**Уникальная особенность — git-first подход:**
```bash
aider --auto-commits   # каждое изменение = коммит
aider --no-auto-commits # только правки без коммитов
```

**Поддержка моделей:**
```bash
aider --model gpt-4o
aider --model claude-opus-4-6
aider --model ollama/qwen2.5-coder:32b
aider --model gemini/gemini-2.5-pro
```

---

## OpenHands (бывший OpenDevin)

**Community** | [github.com/All-Hands-AI/OpenHands](https://github.com/All-Hands-AI/OpenHands)

Полноценный open-source агент с веб-интерфейсом и Docker-изоляцией. Агент работает в изолированном контейнере — не имеет доступа к хост-системе, только к папке проекта.

```bash
docker run -it --rm \
  -e SANDBOX_RUNTIME_CONTAINER_IMAGE=docker.all-hands.dev/all-hands-ai/runtime:latest \
  -v /var/run/docker.sock:/var/run/docker.sock \
  -v ~/.openhands:/home/user/.openhands \
  -p 3000:3000 \
  docker.all-hands.dev/all-hands-ai/openhands:latest
```

**Применение в QA:** запуск в CI как изолированный тест-агент без риска для основной системы.

---

## Сравнительная таблица

| Критерий | Claude Code | Gemini CLI | Qwen Code | Aider |
|----------|-------------|------------|-----------|-------|
| Стоимость | Платный | Бесплатный tier | Бесплатный | Бесплатный (только модель платная) |
| Локальные модели | Нет | Нет | Да (Ollama) | Да |
| MCP-серверы | Да | Да | Да | Нет |
| Субагенты | Да | Нет | Нет | Нет |
| Hooks | Да | Нет | Нет | Нет |
| Git-интеграция | Да | Да | Да | Да (авто-коммит) |
| Открытый код | Нет | Да | Да | Да |
| Изоляция данных | Нет | Нет | Да (локально) | Да (локально) |

---

## Расширение базовых возможностей

### 1. MCP-серверы (Claude Code, Gemini CLI, Qwen Code)

Добавляют новые инструменты: браузер, БД, внешние API, системы управления тестами.

```json
{
  "mcpServers": {
    "playwright":  { "command": "npx", "args": ["@playwright/mcp@latest"] },
    "postgres":    { "command": "npx", "args": ["@modelcontextprotocol/server-postgres"] },
    "github":      { "command": "npx", "args": ["@modelcontextprotocol/server-github"] },
    "jira":        { "command": "npx", "args": ["mcp-server-jira"] }
  }
}
```

### 2. Файлы контекста проекта (CLAUDE.md / GEMINI.md)

Стандартизируют поведение агента в проекте. Хранятся в репозитории, версионируются вместе с кодом.

```markdown
## Для QA-команды

### Как писать тест-кейсы
- Используй формат: Given / When / Then
- Каждый тест независим (нет shared state)
- Тестовые данные — только через фабрики в tests/factories.py

### Как репортить баги
- Severity: Critical/High/Medium/Low
- Обязательные поля: шаги воспроизведения, ожидаемый/фактический результат

### Команды
- `make test`         — все тесты
- `make test-smoke`   — smoke suite
- `make coverage`     — отчёт покрытия
- `make lint`         — линтер
```

### 3. Hooks и автоматизация (Claude Code)

```json
{
  "hooks": {
    "PostToolUse": [{
      "matcher": "Bash",
      "hooks": [{
        "type": "command",
        "command": "if [[ '$CLAUDE_TOOL_OUTPUT' == *'FAILED'* ]]; then echo 'Тесты упали!' >> test_failures.log; fi"
      }]
    }]
  }
}
```

### 4. Custom инструкции через system prompt

Многие инструменты позволяют задать дополнительный system prompt для специализации агента:

```bash
# Claude Code — через CLAUDE.md
# Aider — через --system
aider --system "Ты QA-инженер. Для каждого изменения кода обязательно пиши тест."

# Gemini CLI — через GEMINI.md
```

### 5. CI/CD интеграция

```yaml
# Universal CI pattern (работает с любым агентом)
- name: AI QA Review
  run: |
    # Claude Code
    claude --print "Найди потенциальные баги в изменённых файлах: $(git diff --name-only HEAD~1)" > report.txt

    # Gemini CLI
    gemini -p "Проверь тесты на наличие flaky patterns: $(git diff --name-only HEAD~1 -- '*test*')" > report.txt

    # Qwen Code (локальная модель)
    QWEN_API_BASE=http://ollama:11434 qwen -p "Code review с фокусом на безопасность" > report.txt
```

---

## Паттерны использования для QA

### Паттерн 1: Двойной агент (Code + Test)

```
Разработчик запускает Coding Agent → пишет код
QA запускает Testing Agent → пишет тесты к этому коду
Оба агента работают параллельно на одной кодовой базе
```

### Паттерн 2: Review агент на PR

```
Trigger: новый PR

Gemini CLI / Claude Code:
1. Читает diff
2. Проверяет покрытие тестами
3. Ищет потенциальные баги
4. Комментирует PR с находками
```

### Паттерн 3: Локальный агент для конфиденциального кода

```
Банковское ПО / медицина / госсектор:

Qwen Code + Ollama (локально) → нет отправки данных в облако
Модель: qwen2.5-coder:32b (достаточно для большинства задач)
```

### Паттерн 4: Специализированный QA-агент

```bash
# Запуск агента с QA-специализацией
claude --append-system-prompt "
  Ты QA-инженер. При анализе кода всегда:
  1. Ищи граничные случаи
  2. Проверяй обработку ошибок
  3. Оцени тестируемость кода
  4. Предлагай конкретные тест-кейсы
"
```

---

## Выбор инструмента

**Claude Code** — если нужны максимальные возможности (субагенты, MCP, hooks), и вы работаете с открытым кодом или внешними сервисами.

**Gemini CLI** — если нужен бесплатный доступ к мощной модели (Gemini 2.5 Pro) или важен открытый исходный код.

**Qwen Code** — если код не должен покидать инфраструктуру (финансовый сектор, NDA, enterprise).

**Aider** — если нужна поддержка разных моделей и важна git-интеграция с авто-коммитами.

**OpenHands** — если нужна полная изоляция агента в контейнере.

---

## Связанные материалы

- [Claude Code](claude-code.md)
- [Agentic Development](agentic-development.md)
- [MCP серверы для тестирования](mcp-servery-dlya-testirovaniya.md)
- [REPL-loop](repl-loop.md)
- [Human-in-the-Loop](human-in-the-loop.md)
- [Vibe Coding](vibe-coding.md)
