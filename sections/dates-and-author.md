# Set Commit Date & Author in Git

Sometimes you want to create commits with a specific timestamp — for documentation purposes, contribution graphs, or reconstructing project history.

---

## Initial empty commit with custom date and author

This creates an empty initial commit with a fixed timestamp and author identity:

```bash
git init
export GIT_AUTHOR_DATE="2025-06-21T11:12:56"
export GIT_COMMITTER_DATE="2025-06-21T11:12:56"
git commit --allow-empty -m "chore: initial commit"
```

Tip: Use this if you want your repo to start on a specific date (e.g., symbolic start or matching other tools).

---

## Important Note: `export` affects your entire terminal session

If you use `export`, the date will apply to all subsequent commits in the same terminal window until you close it or manually unset the variables:

```bash
unset GIT_AUTHOR_DATE
unset GIT_COMMITTER_DATE
```

---

## Inline usage (recommended for one-time commits)

To avoid affecting future commits, use this one-liner:

```bash
GIT_AUTHOR_DATE="2025-07-20T07:14:07"
GIT_COMMITTER_DATE="2025-07-20T07:14:07"
git commit -m "feat: add example with backdated commit"
```

Preferred method for retroactive commits. Does not persist in the terminal session.

---

## Update the date of the last commit (after the fact)

If you've already committed and want to change the date:

```bash
git commit --amend --no-edit \
  --date="2025-07-20T07:14:07"
```

Then force-push if already pushed:

```bash
git push --force
```

---

## Change author name and email (for this repo only)

To override the author identity:

```bash
git config user.name "Your Name"
git config user.email "your@email.com"
```

Use `--global` if you want to apply it to all repos on your system.

---

## Verification

To verify the date of your commits:

```bash
git log --pretty=fuller
```

This shows both author and committer date clearly.

---

## Example Use Cases

* Backfilling a contribution graph
* Commemorating symbolic milestones
* Replaying past code states
* Crafting aesthetically ordered timelines

---

You are not just pushing code — you are shaping history.
