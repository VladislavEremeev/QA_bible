---
name: update-page
description: Refresh the content of a «Библия QA» page — tool/OS versions, AI models, prices, statistics, dead or moved links — verified against primary sources. Use for "актуализируй", "обнови", "проверь, не устарело ли".
---

# Refresh a page

Formatting rules and the book contract are in `AGENTS.md`. This skill is about content, not appearance.

## What to look for

* Versions of tools, OSes, languages, APIs that have had a new major release.
* Names and capabilities of AI models and agents.
* Tools that are discontinued, abandoned or renamed.
* Prices, plans, free-tier limits.
* Statistics without a year; undated wording like «сейчас», «на сегодняшний день», «последняя версия».
* Links that don't open or land on a homepage instead of the article.
* Store requirements (App Store / Google Play), standards (ISTQB Glossary, ISO).

Theory pages (testing types and techniques) age slowly — for them check mainly links and examples.

## Steps

1. Read the whole page; list the claims matching the above, with line numbers.
2. For each, find a primary source: official docs, release notes, glossary, RFC. Blogs/Telegram only as corroboration.
3. No source found → don't change or add the claim; report it to the user as "needs human check".
4. Edit minimally: replace the outdated fact, add a year («по данным … 2026», «(на 11.2026)»), replace a dead
   link with the material's new URL or a `web.archive.org` copy. Don't delete links to Russian sites that are
   unreachable from your network without a human check.
5. Don't normalise the file's style (dashes, bold subheadings, list markers stay as in the file).
6. Run the `fact-check` skill on the diff and the claim list; apply its verdict.
7. Report: what changed (with sources), what is unconfirmed, what needs a decision.

Commit only if the user asks; message in Russian: «Актуализировать <тема страницы>». No formatting changes in the same change.
