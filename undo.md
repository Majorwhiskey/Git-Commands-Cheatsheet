# ⏪ Undo Commands

## git restore

Discard unstaged changes in a file:

```bash
git restore file.txt
```

Unstage a file (remove from staging area without losing changes):

```bash
git restore --staged file.txt
```

---

## git reset

Move HEAD back by one commit. Three modes:

**`--soft`** — keeps changes staged:

```bash
git reset --soft HEAD~1
```

**`--mixed`** (default) — keeps changes in working directory but unstages them:

```bash
git reset HEAD~1
```

**`--hard`** — discards all changes permanently:

```bash
git reset --hard HEAD~1
```

> Use `--hard` with caution. Changes are unrecoverable unless found via `git reflog`.

---

## git revert

Undo a commit safely by creating a new commit. Safe to use on shared/public branches.

```bash
git revert <commit_id>
```

---

## When to use what

| Situation | Command |
|---|---|
| Discard file changes | `git restore file.txt` |
| Unstage a file | `git restore --staged file.txt` |
| Undo last commit, keep changes staged | `git reset --soft HEAD~1` |
| Undo last commit, keep changes unstaged | `git reset HEAD~1` |
| Undo last commit, discard all changes | `git reset --hard HEAD~1` |
| Undo a pushed commit safely | `git revert <commit_id>` |

---

## Related

- [advanced.md](advanced.md) – `git reflog` to recover from `--hard` resets
- [basics.md](basics.md) – Core commands
