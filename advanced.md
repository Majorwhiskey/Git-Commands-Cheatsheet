# 🔥 Advanced Commands

## git stash

Temporarily save uncommitted changes:

```bash
git stash
```

Save with a descriptive label:

```bash
git stash push -m "work in progress on login"
```

View all stashes:

```bash
git stash list
```

Apply a specific stash (without removing it):

```bash
git stash apply stash@{0}
```

Pop the most recent stash (apply and remove):

```bash
git stash pop
```

Drop a specific stash:

```bash
git stash drop stash@{0}
```

---

## git cherry-pick

Apply a specific commit to the current branch:

```bash
git cherry-pick <commit_id>
```

---

## git reflog

View history of all HEAD movements — useful for recovering lost commits:

```bash
git reflog
```

Recover a commit after a `--hard` reset:

```bash
git reset --hard <reflog_commit_id>
```

---

## git rebase -i

Interactively edit, squash, reword, or reorder commits:

```bash
git rebase -i HEAD~3
```

---

## git tag

Create a lightweight tag:

```bash
git tag v1.0
```

Create an annotated tag (recommended for releases):

```bash
git tag -a v1.0 -m "Release version 1.0"
```

List all tags:

```bash
git tag
```

Push tags to remote:

```bash
git push origin --tags
```

---

## git bisect

Find the commit that introduced a bug using binary search:

```bash
git bisect start
git bisect bad                  # current commit is broken
git bisect good <commit_id>     # last known good commit
# Git checks out a midpoint — test it, then mark:
git bisect good                 # or: git bisect bad
# Repeat until the culprit commit is found
git bisect reset                # exit bisect mode
```

---

## git clean

Remove untracked files:

```bash
git clean -fd
```

---

## Related

- [undo.md](undo.md) – `git restore`, `git reset`, `git revert`
- [merging.md](merging.md) – Rebase workflow
