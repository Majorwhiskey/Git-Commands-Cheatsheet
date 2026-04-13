# ⏪ Undo Commands

## git restore

Discard changes in a file.

```bash
git restore file.txt
```

## git reset

Move HEAD to undo commits.

```bash
git reset --soft HEAD~1
git reset --hard HEAD~1
```

## git revert

Undo a commit safely by creating a new commit.

```bash
git revert <commit_id>
```
