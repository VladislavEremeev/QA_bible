---
name: review-consistency
description: Read-only review of a «Библия QA» diff against AGENTS.md rules — meaning unchanged, H1/SUMMARY/filename aligned, the file's own style preserved. Use after any page edit, before reporting work as done.
---

# Consistency review

Read-only: don't edit files. Allowed git commands: `git diff`, `git status`, `git show`. Read `AGENTS.md` first.
Best run in a fresh context given only the diff, so earlier conclusions don't bias the review.

Check the diff:

1. **Meaning unchanged** in formatting edits: no lost claims, examples or links; quotes not paraphrased.
2. **Book contract**: new/renamed/deleted pages reflected in `SUMMARY.md`; H1 matches the `SUMMARY.md` title;
   no needless renames; image paths and internal links point to existing files.
3. **File style preserved**: edits don't introduce a foreign style (dashes, subheadings, markers) into a file that
   uses another; everything within the file is consistent.
4. **Language**: Russian prose, English term in parentheses on first mention, official product spelling.
5. Formatting and content not mixed; no pages outside the task touched.

Report: `file:line — problem — how to fix`, blockers separate from suggestions. No remarks — say so.
