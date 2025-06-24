# Working with Branches

This section covers how to create, switch, rename, delete, and manage branches in Git.

---

## Create a New Branch

```bash
git branch feature-xyz
```

Creates a new branch called `feature-xyz` without switching to it.

---

## Create and Switch to a Branch

```bash
git checkout -b feature-xyz
```

Shortcut: creates and immediately switches to the new branch.

---

## Switch to an Existing Branch (modern syntax)

```bash
git switch feature-xyz
```

Modern, safer alternative to `checkout` for switching branches.

---

## Rename the Current Branch

```bash
git branch -m new-branch-name
```

Renames the currently active branch.

---

## Delete a Local Branch

```bash
git branch -d feature-xyz
```

Deletes a local branch. Fails if the branch has unmerged changes.

Force delete:

```bash
git branch -D feature-xyz
```

---

## List All Branches

```bash
git branch
```

Lists all local branches.

---

## List Remote Branches

```bash
git branch -r
```

Lists all remote-tracking branches.

---

## List All Branches (local + remote)

```bash
git branch -a
```

Shows all branches including local and remote.

---

File: `sections/branches.md`
Last updated: 2025-06-22
