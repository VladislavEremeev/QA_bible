---
name: audit
description: Walk a chapter (or the whole book) of «Библия QA» and list freshness and consistency problems — no edits. Use for "что устарело", "составь план приведения в порядок", "проверь раздел".
---

# Audit a chapter

No fixes — findings only.

1. Take the chapter from `SUMMARY.md`. For the whole book go chapter by chapter; for large scope, if the agent
   can run parallel workers, give each a chapter and merge their findings.
2. For each page note:
   * **freshness** — signs from the `update-page` skill (versions, AI, prices, «сейчас», suspicious links);
     last content change: `git log -1 --format=%ad --date=short -- <file>`;
   * **consistency** — signs from the `unify-page` skill (H1 ↔ SUMMARY, mixed style within the file, terms);
   * **book contract** — page missing from `SUMMARY.md`, entry without a file, broken relative paths.
3. Create no files. Return findings as a list `file:line — problem — work type
   (freshness | consistency | contract) — skill`, plus a separate list of items needing the book owner's decision.
4. The `plan-work` skill builds the plan and order of work from this list.
