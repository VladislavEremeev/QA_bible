---
name: sync-upstream
description: Pull changes from the canonical VladislavEremeev/QA_bible (upstream/master) into the fork and check the book isn't broken, including edits made in the GitBook web editor (GITBOOK-N commits). Use for "синхронизируй с upstream", "что нового в оригинале".
---

# Sync with upstream

1. `git fetch upstream`, then `git log --oneline master..upstream/master` — what arrived.
2. `GITBOOK-N` commits are GitBook web-editor edits: review their diffs (`git show <hash>`) for a broken
   `SUMMARY.md`, broken image paths, unclosed `{% hint %}`.
3. List conflicts with the fork's local changes to the user.
4. Merge only after user confirmation (`git merge upstream/master` into the fork's `master`). No rebase, no push.
5. After the merge: every `SUMMARY.md` entry touched by upstream points to an existing file; new upstream files
   are in `SUMMARY.md` (check via `git diff --name-status` and `grep`).
6. Report: what arrived, what broke, which pages should go to `update-page` / `unify-page`.
