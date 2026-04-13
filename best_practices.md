# Best Practices

## Commit Message Rules

* Write clear and meaningful messages
* Use present tense (e.g., "Add feature" not "Added feature")
* Keep messages short but descriptive

Example:

```bash
git commit -m "Add login validation"
```

---

## Branching Strategy

* Never work directly on the main branch
* Use feature branches for new work
* Use descriptive branch names

Examples:

* feature/user-auth
* bugfix/login-error
* docs/update-readme

---

## Avoiding Conflicts

* Pull latest changes before starting work
* Commit frequently
* Keep branches small and focused
* Communicate with team members

---

## General Tips

* Use `git status` frequently
* Review changes before committing (`git diff`)
* Avoid using `git reset --hard` unless necessary
* Keep your repository clean and organized
