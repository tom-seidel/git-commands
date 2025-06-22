# Git Basics

Essential Git commands for initializing and managing a local repository.

Use this section when you're starting from scratch or need a quick reminder of the core workflow.

---

## Initialize a Repository

```bash
git init
```

Creates a new `.git` folder and starts version control in the current directory.

---

## Track Changes

### Add everything:

```bash
git add .
```

### Add specific file:

```bash
git add filename.txt
```

### Check what's staged & unstaged:

```bash
git status
```

---

## Make a Commit

```bash
git commit -m "feat: add something new"
```

Records a snapshot of your staged files. Use clear, meaningful commit messages.

---

## View History

```bash
git log
```

Shows all previous commits (long format).

```bash
git log --oneline
```

Shorter format — great for quick overviews.

---

## See Differences

### What's changed but not staged:

```bash
git diff
```

### What's staged (ready to commit):

```bash
git diff --cached
```

---

## Typical Workflow (Local Only)

```bash
git init
git add .
git commit -m "chore: initial commit"
```

---

## .gitignore

Create a `.gitignore` file to exclude files/folders from being tracked:

Example:

```
node_modules/
.env
.DS_Store
dist/
```

---

File: `sections/basics.md`
Last updated: 2025-06-19
