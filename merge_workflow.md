# 🔁 Merge Workflow

Merging is the process of combining changes from one branch into another.

## Types of Merge

### Fast-Forward Merge

When the target branch has no new commits since the feature branch was created, Git simply moves the pointer forward. No merge commit is created.

```bash
git merge feature-branch
```

### No-Fast-Forward Merge

Forces a merge commit even when fast-forward is possible. Preserves the fact that a feature branch existed — useful for traceability in team projects.

```bash
git merge --no-ff feature-branch
```

### Squash Merge

Collapses all commits from the feature branch into a single commit on the target branch. Keeps history clean.

```bash
git merge --squash feature-branch
git commit -m "Add feature X"
```

### Rebase (Alternative to Merge)

Replays commits on top of another branch for a linear history:

```bash
git rebase main
```

---

## Pull Request Merge

1. A pull request is reviewed
2. Maintainer approves changes
3. Changes are merged into the main branch (via merge commit, squash, or rebase depending on team preference)

---

## Handling Conflicts

If conflicts occur during a merge:

1. Git marks conflicting sections in the file
2. Manually edit the file to resolve
3. Stage the resolved file and commit:

```bash
git add .
git commit
```

To cancel the merge entirely:

```bash
git merge --abort
```

---

## Notes

- Always pull latest changes before merging
- Prefer `--no-ff` in team environments to keep branch history visible
- Resolve conflicts carefully to avoid breaking code

---

## Related

- [merging.md](merging.md) – Merge and rebase commands
- [branching.md](branching.md) – Managing branches
- [pull_request.md](pull_request.md) – Pull request workflow
