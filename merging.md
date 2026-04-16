# 🔀 Merging & Rebase

## git merge

Combine another branch into the current branch:

```bash
git merge feature
```

Force a merge commit even when fast-forward is possible (preserves branch history):

```bash
git merge --no-ff feature
```

Squash all commits from the branch into one (does not auto-commit):

```bash
git merge --squash feature
git commit -m "Add feature X"
```

---

## git rebase

Reapply commits on top of another branch for a cleaner, linear history:

```bash
git rebase main
```

Continue after resolving a conflict during rebase:

```bash
git rebase --continue
```

---

## git merge --abort

Cancel a merge in case of conflicts:

```bash
git merge --abort
```

---

## git rebase --abort

Stop an ongoing rebase process:

```bash
git rebase --abort
```

---

## Merge vs Rebase

| | Merge | Rebase |
|---|---|---|
| History | Preserves branch history | Creates linear history |
| Commits | Adds a merge commit | Replays commits |
| Use when | Shared branches, PRs | Local cleanup before pushing |

---

## Related

- [branching.md](branching.md) – Creating branches
- [merge_workflow.md](merge_workflow.md) – Team merge workflow
- [advanced.md](advanced.md) – Interactive rebase
