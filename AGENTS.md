# AGENTS.md

Instructions for any AI coding agent working in this repository. Format: [agents.md](https://agents.md).
The repository is vendor-neutral by design: no tool-specific instruction files or directories — only this file
and `.agents/skills/`.

## What this repository is

"Библия QA" — a Russian-language QA knowledge base (~235 pages) published as a GitBook at
https://vladislaveremeev.gitbook.io/qa_bible/. There is **no code, no build, no test suite, no
package manager and no CI** — the repository is pure GitBook-flavoured Markdown. "Working in this
repo" means editing content and keeping the navigation consistent.

Local verification is limited to reading the Markdown and checking link/path integrity (e.g. with
`grep`/`find`); rendering happens on GitBook's side after a push to `master`.

This checkout is a fork: `origin` is `iampopovich/QA_bible`, `upstream` is
`VladislavEremeev/QA_bible` (the canonical repo whose `master` feeds the published book). Upstream
content arrives via merge commits from `upstream/master`, so prefer small, additive changes that
merge cleanly.

## Structure and the SUMMARY.md contract

Top-level directories are the book's chapters (`obshee`, `vidy-metody-urovni-testirovaniya`,
`test-dizain`, `seti-i-okolo-nikh`, `mobilnoe-testirovanie`, `avtomatizaciya-testirovaniya`,
`ai-v-testirovanii`, …). Each holds one `README.md` (the chapter landing page, usually just a
heading and a short intro) plus one flat `*.md` file per topic. There is no deeper nesting.

`SUMMARY.md` is the single source of truth for navigation — GitBook renders the sidebar from it,
and a page absent from `SUMMARY.md` is effectively invisible. **Any new, renamed, moved or deleted
page requires the matching edit in `SUMMARY.md` in the same commit.** Its format:

- top-level `* [Title](dir/README.md)` for a chapter, with its pages indented two spaces below;
- a plain indented line with no link (e.g. `  * Основы` under `avtomatizaciya-testirovaniya`) is a
  non-clickable grouping label; its pages are indented one level further. Only this chapter
  currently uses groups.

Images live in `.gitbook/assets/` (filenames may contain spaces and Cyrillic) and are referenced
with a relative path from the page, e.g. `.gitbook/assets/logcat.png`. Embed them with GitBook's
`<figure><img src="..." alt=""><figcaption></figcaption></figure>` markup.

## Content conventions

- **Language**: all prose, headings and `SUMMARY.md` titles are in Russian. Technical terms are
  given with the English original in parentheses — both in page titles and in filenames, e.g.
  `testirovanie-metodom-chernogo-yashika-black-box-testing.md` →
  `Тестирование методом черного ящика (Black Box Testing)`.
- **Filenames**: lowercase kebab-case ASCII transliteration of the Russian title, English term
  appended. Keep the filename and the `# H1` of the page in sync; the `SUMMARY.md` title should
  match the H1.
- **Page shape**: one `# H1` matching the title, then body. Sub-sections are frequently written as
  bold lines (`**Структура HTTP-сообщения**`) rather than `##` headings — follow whatever the file
  being edited already does instead of normalising it.
- **Callouts**: `{% hint style="info" %} … {% endhint %}` (also `danger`, `warning`, `success`) for
  notes and caveats. Used sparingly, mostly in `ai-v-testirovanii`.
- **Dashes**: the existing text uses a plain hyphen surrounded by spaces (` - `) where Russian
  typography would want an em dash; some newer pages use ` — `. Match the file.
- The book is explicitly a reference collection ("копилка, а не учебник"), not a tutorial — write
  reference prose with links to primary sources, not step-by-step lessons.

`CONTRIBUTING.md` is a placeholder ("coming soon"); these conventions are derived from the existing
content and are the de facto contribution rules.

## Agent artifacts

Markdown only, no scripts. Use them for maintenance tasks instead of improvising.

**Skills** — `.agents/skills/<name>/SKILL.md` ([Agent Skills](https://agentskills.io) open format). If your agent
doesn't load skills automatically, open the matching `SKILL.md` and follow it.

Coordination:

- `plan-work` — entry point for anything bigger than one page: splits the request into tasks (one chapter or
  ≤ ~10 pages, one work type), assigns skills and reviews, keeps the plan in the session — never in plan files.

Execution:

- `audit` — walk a chapter, return findings, no edits;
- `update-page` — refresh content against primary sources;
- `unify-page` — consistency within the file's own style;
- `add-page` — new page plus `SUMMARY.md` entry;
- `sync-upstream` — merge `upstream/master`, review `GITBOOK-N` web-editor commits.

Review (read-only):

- `fact-check` — every changed claim against a primary source;
- `review-consistency` — the diff against the rules in this file.

Review is mandatory after edits: `review-consistency` always, `fact-check` for freshness updates and new pages.
If the agent can run isolated workers, run reviews in a fresh one given only the diff, not your conclusions.

## Boundaries

- No commits or pushes unless the user asks. Commit messages in Russian, imperative; formatting-only commits start
  with `Оформление:`, content refreshes with `Актуализировать …`. Formatting and content in separate commits.
- Never rename or move existing pages (filename = public URL) and no book-wide mass replacements — escalate.
- Don't invent facts, versions or links: no source — no claim.
