# ⚡ Quick Git Cheatsheet

## Setup

```bash
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
```

## Daily Workflow

```bash
git status
git add .
git commit -m "msg"
git pull
git push
```

## Branching

```bash
git checkout -b feature     # create + switch
git switch feature          # switch (modern)
git branch -d feature       # delete (safe)
git branch -D feature       # delete (force)
```

## Remotes

```bash
git remote add origin <url>
git remote -v
git fetch origin
git pull origin main
git push -u origin feature
git push origin --delete feature
```

## Undo

```bash
git restore file             # discard unstaged changes
git restore --staged file    # unstage a file
git reset HEAD~1             # undo last commit (keep changes)
git reset --hard HEAD~1      # undo last commit (discard changes)
git revert <id>              # safe undo (creates new commit)
```

## Merge & Rebase

```bash
git merge feature
git merge --no-ff feature    # force merge commit
git merge --squash feature   # squash into one commit
git rebase main
git rebase -i HEAD~3         # interactive rebase
```

## Advanced

```bash
git stash                    # save work temporarily
git stash list               # view stashes
git stash pop                # restore latest stash
git cherry-pick <id>         # apply specific commit
git reflog                   # view HEAD history
git tag -a v1.0 -m "msg"     # create annotated tag
git bisect start             # start bug hunt
```
