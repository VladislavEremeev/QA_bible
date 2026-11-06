---
name: plan-work
description: Plan and coordinate multi-step changes in «Библия QA» — refresh a chapter, make the book consistent, sync with upstream. Splits the request into tasks, assigns skills and reviews, tracks completion; keeps the plan in the session, never in files. Use for any request bigger than a single page.
---

# Plan and coordinate work

Book rules are in `AGENTS.md` — read it first. Don't edit pages directly when a skill below covers the work.

## Executors

| Work | Skill |
|---|---|
| Walk a chapter, find problems | `audit` (no edits) |
| Content freshness | `update-page` |
| Consistency, proofreading | `unify-page` |
| New page | `add-page` |
| Upstream sync | `sync-upstream` |
| Fact check (read-only) | `fact-check` |
| Diff review against rules (read-only) | `review-consistency` |

## Where the plan lives

In the session: the agent's task list if it has one, otherwise a numbered list in the conversation.
Never create plan files in the repo. If work is unfinished at session end, give the user a short
"done / remaining / awaiting decision" summary — enough to resume, since book state is recovered from the pages
and `git status`, not from an old plan.

## Workflow

1. **Scope.** Which chapter (per `SUMMARY.md`), which work type: freshness or consistency. More than one chapter →
   start with `audit` per chapter.
2. **Plan.** Task = one chapter or up to ~10 pages and **one** work type. Per task: pages, skill, done criterion.
   Order: broken book contract (`SUMMARY.md`, broken paths) → fast-ageing topics (AI, tools, links, mobile OS) →
   the rest. Show the plan to the user and wait for approval before changing files.
3. **Execute one task at a time** with its skill. After edits run `review-consistency` on the diff, plus
   `fact-check` for freshness and new pages. If the agent can run isolated workers, run reviews in a fresh worker
   given only the diff — not your conclusions. Blockers go back to the task; unresolvable ones to "awaiting decision".
4. **Close a task** only after review passes. Don't start the next until the current one is closed.
5. **Report:** what changed (per page), what was checked, what awaits the book owner's decision.

## Boundaries

* No commits, no pushes unless asked. One task — one commit; formatting and content separate.
* Never rename or move pages, no book-wide replacements — escalate.
* Independent tasks in different chapters may run in parallel; edits to one file strictly sequential.
