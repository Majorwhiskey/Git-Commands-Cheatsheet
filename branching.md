# 🌿 Branching Commands

## git branch

List local branches:

```bash
git branch
```

List remote branches:

```bash
git branch -r
```

List all branches (local + remote):

```bash
git branch -a
```

Create a new branch without switching:

```bash
git branch feature
```

Rename a branch:

```bash
git branch -m old-name new-name
```

---

## git checkout

Switch to an existing branch:

```bash
git checkout feature
```

Create and switch to a new branch:

```bash
git checkout -b feature
```

---

## git switch

Modern way to switch branches:

```bash
git switch feature
```

Create and switch to a new branch (modern equivalent of `checkout -b`):

```bash
git switch -c feature
```

---

## git branch -d / -D

Delete a branch safely (only if fully merged):

```bash
git branch -d feature
```

Force-delete a branch regardless of merge status:

```bash
git branch -D feature
```

---

## Delete a Remote Branch

```bash
git push origin --delete feature
```

---

## Related

- [basics.md](basics.md) – Core commands
- [merging.md](merging.md) – Merging branches
- [merge_workflow.md](merge_workflow.md) – Team merge workflow
