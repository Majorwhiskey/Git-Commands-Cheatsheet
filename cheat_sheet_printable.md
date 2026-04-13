# Git Cheat Sheet (Quick Revision)

## Setup

```bash
git init
git clone <url>
```

---

## Basic Workflow

```bash
git status
git add .
git commit -m "message"
git push
git pull
```

---

## Branching

```bash
git branch
git checkout -b feature
git switch feature
git branch -d feature
```

---

## Merging

```bash
git merge feature
git rebase main
```

---

## Undo

```bash
git restore file
git reset HEAD~1
git revert <commit>
```

---

## Advanced

```bash
git stash
git stash pop
git cherry-pick <commit>
git reflog
git clean -fd
```

---

## Remote

```bash
git remote -v
git push -u origin branch
git fetch
```

---

## Key Flow

Edit → Add → Commit → Push → Pull → Merge

---

This sheet is intended for quick revision and daily usage.
