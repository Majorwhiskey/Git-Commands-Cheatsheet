# Merge Workflow

Merging is the process of combining changes from one branch into another.

## Types of Merge

### Standard Merge

Combines branches and preserves history.

```bash
git merge feature-branch
```

### Rebase (Alternative)

Applies commits on top of another branch for cleaner history.

```bash
git rebase main
```

## Pull Request Merge

1. A pull request is reviewed
2. Maintainer approves changes
3. Changes are merged into the main branch

## Handling Conflicts

If conflicts occur:

* Git will mark conflicting sections
* Manually edit the file
* Then run:

```bash
git add .
git commit
```

## Notes

* Always pull latest changes before merging
* Resolve conflicts carefully to avoid breaking code
