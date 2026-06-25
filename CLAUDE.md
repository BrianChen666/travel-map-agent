# Git Version Control Rules

All work in this project must be tracked with git. Follow these rules on every change.

## Commit Discipline

- Commit after every meaningful unit of work — never accumulate unrelated changes in one commit.
- Stage specific files by name (`git add <file>`), never `git add -A` or `git add .`.
- Always write a commit message. Format: `<type>: <short description>` (under 72 chars).
- Allowed types: `feat`, `fix`, `refactor`, `style`, `docs`, `chore`, `test`.
- Push to `origin main` after each commit unless the user says otherwise.

## Before Starting Any Task

1. Run `git status` to confirm the working tree is clean.
2. Run `git pull origin main` to ensure local is up to date.

## After Completing Any Task

1. `git add <changed files>`
2. `git commit -m "<type>: <description>"`
3. `git push origin main`

## Forbidden Actions (never do without explicit user approval)

- `git push --force`
- `git reset --hard`
- `git commit --amend` on already-pushed commits
- `git rebase` on shared branches
- Skipping hooks with `--no-verify`
- Deleting branches without user confirmation

## Commit Message Examples

```
feat: add interactive map component
fix: correct marker coordinate parsing
docs: update README with setup instructions
chore: add .gitignore for node_modules
refactor: extract API call into separate module
```
