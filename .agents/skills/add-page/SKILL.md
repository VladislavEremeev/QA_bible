---
name: add-page
description: Add a new page to «Библия QA» — file in the right chapter, H1, SUMMARY.md entry, sources. Use when asked to write a new article or topic.
---

# New page

1. Make sure the topic doesn't exist: `grep -rli '<term>' --include=*.md .`. If it does — propose extending that page.
2. Chapter — the matching top-level directory (no deeper nesting). Style reference — 1–2 neighbouring pages in the
   same chapter: copy their look (subheadings, dashes, lists).
3. Filename — kebab-case transliteration of the Russian title + English term
   (`testirovanie-metodom-chernogo-yashika-black-box-testing.md`). H1 — `Русский термин (English Term)`.
4. Reference prose («копилка, а не учебник»): definition, essence, examples, links to primary sources.
   Non-obvious claims only with a source; fast-changing facts with a year.
5. Add the `SUMMARY.md` line in the right place (2-space indent per level, one more inside a group) in the same
   change. If the chapter README lists its pages — add it there too.
6. Run the `fact-check` and `review-consistency` skills on the page.
7. Report: path, place in the TOC, sources.
