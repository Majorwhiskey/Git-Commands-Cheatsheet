# Fork

A fork is a personal copy of another repository under your own account. It allows you to experiment and make changes without affecting the original project.

## Why Fork?

* To contribute to open-source projects
* To safely experiment with code
* To work independently from the original repository

## Basic Workflow

1. Fork the repository on GitHub
2. Clone your fork locally

```bash
git clone https://github.com/your-username/repo.git
```

3. Add original repository as upstream

```bash
git remote add upstream https://github.com/original-owner/repo.git
```

4. Sync with upstream

```bash
git fetch upstream
git merge upstream/main
```

## Notes

* Always keep your fork updated with the original repository
* Avoid making changes directly on the main branch
