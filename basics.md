# 🟢 Basic Git Commands

## git config

Set your identity before making commits.

```bash
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
```

View current config:

```bash
git config --list
```

---

## git init

Initialize a new Git repository.

```bash
git init
```

---

## git clone

Copy an existing repository to your local system.

```bash
git clone <repo_url>
```

Clone into a specific folder:

```bash
git clone <repo_url> my-folder
```

---

## git status

Show current changes and staging status.

```bash
git status
```

---

## git add

Stage a specific file:

```bash
git add file.txt
```

Stage all changes:

```bash
git add .
```

Stage parts of a file interactively:

```bash
git add -p file.txt
```

---

## git commit

Save staged changes with a message.

```bash
git commit -m "message"
```

Stage and commit tracked files in one step:

```bash
git commit -am "message"
```

---

## git diff

View unstaged changes:

```bash
git diff
```

View staged changes (what will be committed):

```bash
git diff --staged
```

---

## git log

View commit history:

```bash
git log --oneline
```

View with branch graph:

```bash
git log --oneline --graph --all
```

View changes introduced by each commit:

```bash
git log -p
```

---

## git remote

Add a remote:

```bash
git remote add origin <repo_url>
```

View configured remotes:

```bash
git remote -v
```

---

## git push

Push your branch to the remote:

```bash
git push origin main
```

Push and set upstream (first push of a new branch):

```bash
git push -u origin feature
```

---

## git pull

Fetch and merge the latest changes from the remote:

```bash
git pull origin main
```

---

## git fetch

Download changes from the remote without merging:

```bash
git fetch origin
```

---

## .gitignore

A `.gitignore` file tells Git which files to ignore (logs, build output, secrets, etc.).

Create a `.gitignore` in your project root:

```
# Ignore log files
*.log

# Ignore node_modules
node_modules/

# Ignore environment files
.env
```

Check what is being ignored:

```bash
git status --ignored
```

---

## Related

- [branching.md](branching.md) – Creating and managing branches
- [undo.md](undo.md) – Undoing changes
- [cheatsheet.md](cheatsheet.md) – Quick reference
