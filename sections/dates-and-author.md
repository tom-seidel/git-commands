# Create a commit with a specific date

If you want to create an empty initial commit with a fixed date and author info (for contribution graph or documentation):

```bash
git init
export GIT_AUTHOR_DATE="2025-06-21T11:12:56"
export GIT_COMMITTER_DATE="2025-06-21T11:12:56"
git commit --allow-empty -m "initial commit"
