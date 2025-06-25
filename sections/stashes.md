# Working with Stashes

This section covers how to temporarily store changes using Git stash, and how to re-apply or manage those changes later.

---

## Stash Current Changes

```bash
git stash
```

Saves all tracked but uncommitted changes and restores a clean working directory.

---

## Stash with a Message

```bash
git stash push -m "WIP: fixing navbar layout"
```

Adds a descriptive label to your stash.

---

## List Stashes

```bash
git stash list
```

Displays all saved stashes.

---

## Show Stash Details

```bash
git stash show -p stash@{0}
```

Shows what was changed in a specific stash.

---

## Apply the Latest Stash

```bash
git stash apply
```

Reapplies the most recent stash, but **keeps** it in the stash list.

---

## Apply and Drop (Pop) the Latest Stash

```bash
git stash pop
```

Reapplies the most recent stash and **removes** it from the list.

---

## Drop a Specific Stash

```bash
git stash drop stash@{0}
```

Deletes a specific stash entry.

---

## Clear All Stashes

```bash
git stash clear
```

Removes all stashes.

---

File: `sections/stashing.md`
Last updated: 2025-06-25
