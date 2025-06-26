# Git Command Examples

This file contains real-world examples and common Git workflows, combining multiple commands into practical use cases.

---

## Rebase a Feature Branch onto `main`

```bash
git checkout feature/new-ui
git fetch origin
git rebase origin/main
```

Keeps history linear by replaying your changes on top of the latest `main`.

---

## Undo Last Commit (keep changes)

```bash
git reset --soft HEAD~1
```

Moves HEAD back one commit, but keeps your changes in the staging area.

---

## Remove Last Commit (discard changes)

```bash
git reset --hard HEAD~1
```

Deletes the last commit completely, including all changes.

---

## Force Push After Rewriting History

```bash
git push --force
```

Required after a `rebase` or `reset` that rewrites history.

---

## Clone and Checkout a Specific Branch

```bash
git clone -b feature/landing-page https://github.com/user/repo.git
```

Clones the repo and checks out the specified branch directly.

---

## Create an Empty Commit (e.g. for GitHub contribution graph)

```bash
git commit --allow-empty -m "chore: trigger GitHub activity"
```

---

## Reset Local Branch to Remote

```bash
git fetch origin
git reset --hard origin/main
```

Restores your local branch to match the latest state of the remote.

---

## Remove a File from Git Without Deleting It Locally

```bash
git rm --cached path/to/file.txt
```

Use this when you want Git to stop tracking a file.

---

File: `sections/examples.md`
Last updated: 2025-06-26
