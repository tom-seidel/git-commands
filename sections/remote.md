# Working with Remotes

This section covers how to connect your local repository to a remote one (e.g. GitHub), push and pull changes, and manage remote URLs.

---

## Add a Remote Repository

```bash
git remote add origin https://github.com/your-username/your-repo.git
```

Adds a remote called `origin` pointing to the provided URL.

---

## Push to Remote (First Time)

```bash
git push -u origin main
```

Pushes the current branch to the remote `origin` and sets the upstream branch.

---

## Push to Remote (Later)

```bash
git push
```

Pushes changes to the already set upstream branch.

---

## Pull from Remote

```bash
git pull
```

Fetches and merges changes from the remote tracking branch.

---

## Fetch Without Merge

```bash
git fetch origin
```

Downloads changes from the remote but does not merge them.

---

## View Remote URLs

```bash
git remote -v
```

Shows the remote URLs associated with the current repository.

---

## Change Remote URL

```bash
git remote set-url origin https://github.com/your-username/new-repo.git
```

Changes the URL of the existing remote `origin`.

---

File: `sections/remote.md`
Last updated: 2025-06-23
