# 📬 Pull Request

A pull request (PR) is a request to merge your changes into another repository, typically the original project.

## Purpose

- Share your changes with project maintainers
- Enable code review and discussion
- Ensure code quality before merging

---

## Steps to Create a PR

1. Create a new branch:

```bash
git checkout -b feature-update
```

2. Make changes and commit:

```bash
git add .
git commit -m "Describe your changes"
```

3. Push to your fork:

```bash
git push origin feature-update
```

4. On GitHub:
   - Click **"Compare & Pull Request"**
   - Add a clear title and description
   - Link any related issues (e.g. `Closes #42`)
   - Submit the pull request

---

## PR Best Practices

- Keep PRs small and focused on a single change
- Write a clear description explaining *what* and *why*
- Reference related issues or tickets
- Respond to review comments promptly
- Don't force-push after a review has started

---

## After the PR is Merged

Update your local main branch:

```bash
git checkout main
git pull origin main
```

Delete the feature branch:

```bash
git branch -d feature-update
git push origin --delete feature-update
```

---

## Related

- [fork.md](fork.md) – Forking a repository
- [merge_workflow.md](merge_workflow.md) – How merging works in teams
- [branching.md](branching.md) – Branch management
