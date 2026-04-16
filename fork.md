# 🍴 Fork

A fork is a personal copy of another repository under your own account. It allows you to experiment and make changes without affecting the original project.

## Why Fork?

- To contribute to open-source projects
- To safely experiment with code
- To work independently from the original repository

---

## Basic Workflow

1. Fork the repository on GitHub

2. Clone your fork locally:

```bash
git clone https://github.com/your-username/repo.git
```

3. Add the original repository as upstream:

```bash
git remote add upstream https://github.com/original-owner/repo.git
```

4. Verify remotes:

```bash
git remote -v
```

---

## Syncing with Upstream

Option 1 — Merge:

```bash
git fetch upstream
git merge upstream/main
```

Option 2 — Rebase (cleaner, linear history):

```bash
git fetch upstream
git rebase upstream/main
```

---

## Notes

- Always keep your fork updated with the original repository before opening a PR
- Avoid making changes directly on the main branch
- Use `git fetch upstream` regularly to stay in sync

---

## Related

- [pull_request.md](pull_request.md) – Creating pull requests from your fork
- [branching.md](branching.md) – Branch management
