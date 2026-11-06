---
name: unify-page
description: Make a «Библия QA» page or chapter consistent without changing meaning — H1, filename, SUMMARY entry, terminology, formatting within the file's established style, typos. Use for "приведи к единому виду", "вычитай", "поправь оформление".
---

# Make a page consistent

Rules come from `AGENTS.md` (SUMMARY.md contract, filenames, H1, language, callouts, dashes).
Key principle from it: **follow the file's own style; don't normalise the book to a single template.**

## What to fix

* **H1 ↔ filename ↔ `SUMMARY.md`.** One `# H1` on the first line; the `SUMMARY.md` title matches the H1 (may be
  shorter). Never rename the file — the filename is the page URL; report filename mismatches to the user.
* **Terminology.** Russian term with the English original in parentheses on first mention; one concept has one
  name on the page; products in official spelling (JavaScript, GitHub, PostgreSQL).
* **Consistency inside the file:** if subsections are bold lines — all bold; if `##` — all `##`. Dashes as the
  file predominantly uses (` - ` or ` — `). One list marker per file.
* **Callouts** `{% hint %}` opened and closed; style one of `info / warning / danger / success`.
* **Images** from `.gitbook/assets/` via relative path, inside `<figure>`.
* **Typos and punctuation** — clear errors only («тест кейс» → «тест-кейс», «так же» → «также» where meant).

## Don't

* Change meaning, shorten or reorder material — propose that to the user as a list instead.
* Paraphrase quotes and ISTQB definitions.
* Do book-wide replacements (dashes, «ё», quotes) — only within the pages being processed.
* Touch GitBook markup beyond what's needed.

## Steps

1. Read the page and its `SUMMARY.md` line; determine the file's predominant style.
2. Make the edits. Scope per run: one chapter or up to ~10 pages.
3. Verify every link and image path you touched exists (`grep`/`find`).
4. Run the `review-consistency` skill on the diff; apply its remarks.
5. Report: what was fixed, what was left and why, what is proposed separately.

Commit only if asked; message «Оформление: <страница или раздел>», no content changes in it.
