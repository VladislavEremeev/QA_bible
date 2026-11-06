---
name: fact-check
description: Read-only fact check of a «Библия QA» page or diff — definitions, versions, tool capabilities, numbers, source links. Use after refreshing content or adding a page, or when asked "проверь факты".
---

# Fact check

Read-only: don't edit files. Allowed git commands: `git diff`, `git show`, `git log`. Needs web access.
Best run in a fresh context given only the diff or file path, so earlier conclusions don't bias the check.

For each claim (diff lines; if given a file — the whole page):

1. Find a primary source: official docs, release notes, ISTQB Glossary, RFC, standard.
2. Check the page's links open and actually support the text, not a homepage.
3. Versions, prices, models, statistics — is there a year, and is it true today.
4. ISTQB definitions must match the glossary and not be distorted by paraphrase.

Report as a table `line | claim | correct / outdated / wrong / unconfirmed | source`, then: what to fix and what
needs a human decision. Never invent sources: if not found — "unconfirmed".
