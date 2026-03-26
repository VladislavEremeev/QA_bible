# Мутационное тестирование (Mutation Testing)

Юнит-тесты помогают убедиться, что код работает так, как мы хотим. Но насколько сами тесты надёжны? Если удалить все `assert`-строки или заменить их на `assertSame(1, 1)`, code coverage останется 100% — а тесты не проверят ничего. Мутационное тестирование отвечает на вопрос: «Насколько хороши наши тесты?»

## Определение

**Мутационное тестирование (Mutation Testing)** — вид тестирования методом белого ящика, при котором в исходный код намеренно вносятся небольшие изменения (мутации), после чего проверяется, упадут ли существующие тесты. Если тесты проходят несмотря на изменение логики — тест-суит неэффективен.

Ключевая метрика — **Mutation Score Indicator (MSI)**:
```
MSI = Killed Mutants / Valid Mutants × 100%
```

Цель — максимально высокий MSI: большинство мутантов должны быть «убиты» тестами.

## Типы мутаций

* **Мутация значений (Value mutation)** — изменение константы или параметра (`5` → `0`)
* **Мутация операторов (Statement mutation)** — удаление или замена оператора (`return x` → `return null`)
* **Мутация решения (Decision mutation)** — замена логических операторов (`>` → `>=`, `&&` → `||`)

## Виды мутантов

* **Убитые (Killed)** — тест упал после мутации; хорошо, тест работает
* **Выжившие (Survived)** — тест прошёл несмотря на мутацию; плохо, нужна дополнительная проверка
* **Эквивалентные (Equivalent)** — мутация не меняет поведение программы; не влияют на MSI
* **Timeout** — мутант привёл к бесконечному циклу; считается обнаруженным
* **Нет покрытия (No Coverage)** — мутант в коде, не покрытом тестами

## Инструменты мутационного тестирования

### Stryker (JavaScript / TypeScript)

**Stryker** — самый популярный инструмент мутационного тестирования для JavaScript/TypeScript. Поддерживает Jest, Mocha, Karma, Jasmine. Генерирует детальные HTML-отчёты с диффом мутаций.

```bash
npm install --save-dev @stryker-mutator/core @stryker-mutator/jest-runner
npx stryker run
```

```json
// stryker.config.json
{
  "testRunner": "jest",
  "mutate": ["src/**/*.ts", "!src/**/*.spec.ts"],
  "reporters": ["html", "clear-text", "progress"],
  "thresholds": { "high": 80, "low": 60, "break": 50 }
}
```

Особенности:
* Инкрементальный режим — пересчитывает только мутантов в изменённых файлах
* Поддержка TypeScript, JavaScript, React, Vue
* Dashboard для отслеживания MSI в CI

### PIT / Pitest (Java)

**PIT** — стандарт мутационного тестирования для Java. Работает на уровне байткода (не исходников), что делает его существенно быстрее подходов на основе перекомпиляции. Интеграция с Maven и Gradle.

```xml
<!-- Maven plugin -->
<plugin>
  <groupId>org.pitest</groupId>
  <artifactId>pitest-maven</artifactId>
  <version>1.15.0</version>
  <dependencies>
    <dependency>
      <groupId>org.pitest</groupId>
      <artifactId>pitest-junit5-plugin</artifactId>
    </dependency>
  </dependencies>
</plugin>
```

```bash
mvn test-compile org.pitest:pitest-maven:mutationCoverage
```

Особенности:
* Работает с JUnit 4, JUnit 5, TestNG
* Параллельный анализ мутантов
* Интеграция с SonarQube

### mutmut (Python)

**mutmut** — простой CLI-инструмент для Python. Минимальная настройка, хорошая интеграция с pytest.

```bash
pip install mutmut
mutmut run  # запустить мутационное тестирование
mutmut results  # посмотреть результаты
mutmut show 5   # показать конкретного мутанта
```

```bash
# Применить выжившего мутанта для изучения
mutmut apply 5
pytest tests/  # убедиться что тест не падает
mutmut revert  # откатить мутацию
```

Особенности:
* Кэширует результаты между запусками
* Подробный вывод: какие строки выжили
* [Хорошая статья на Habr](https://habr.com/ru/company/vdsina/blog/512630/)

### Сравнение инструментов

| Инструмент | Язык | Интеграция | Скорость | Отчёты |
|---|---|---|---|---|
| **Stryker** | JS/TS | Jest, Mocha, Karma | Средняя (AST) | HTML + Dashboard |
| **PIT** | Java | Maven, Gradle, JUnit | Быстрая (байткод) | HTML + XML |
| **mutmut** | Python | pytest | Медленная (исходники) | CLI + JSON |
| **Infection** | PHP | PHPUnit | Средняя | HTML + Text |

## Место в CI/CD

Мутационное тестирование ресурсоёмко — полный прогон на большой кодовой базе занимает часы. Рекомендуемый подход:
* Запускать инкрементально (только изменённые файлы) в PR
* Полный прогон — по расписанию (ночной/weekly)
* Установить пороги в конфиге (Stryker `thresholds`) и падать при снижении MSI

## Источники

* [Stryker Mutator — документация](https://stryker-mutator.io/docs/)
* [PIT (Pitest) — документация](https://pitest.org)
* [mutmut — документация](https://mutmut.readthedocs.io)
* [Мутационное тестирование](https://habr.com/ru/post/334394/)
* [Изучаем mutmut](https://habr.com/ru/company/vdsina/blog/512630/)

### Дополнительные материалы

* [Mutation Testing (Google Testing Blog)](https://testing.googleblog.com/2021/04/mutation-testing.html) — как Google применяет мутационное тестирование
* [What Is Mutation Testing: Tutorial With Examples](https://www.softwaretestinghelp.com/what-is-mutation-testing/) — подробный гайд
