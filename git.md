# 🔄 Git Cheatsheet

## Basic Commands

```bash
git init                    # Initialize new repo
git clone <url>             # Clone a repo
git status                  # Show status
git add .                   # Stage all changes
git commit -m "message"     # Commit changes
git push                    # Push to remote
git pull                    # Pull from remote
```

## Branch Operations

```bash
git branch                  # List branches
git checkout -b <branch>    # Create and switch branch
git switch <branch>         # Switch branch
git merge <branch>          # Merge branch
git branch -d <branch>      # Delete branch
```

## Undo Operations

```bash
git reset --soft HEAD~1     # Undo last commit (keep changes)
git reset --hard HEAD~1     # Undo last commit (discard changes)
git stash                   # Stash changes
git stash pop               # Apply stashed changes
```

## Log and Diff

```bash
git log --oneline           # Short log
git log --graph             # Graph log
git diff                    # Show changes
git diff --staged           # Show staged changes
```

## Tips

```bash
git commit -m "fix: bug fix"  # Conventional commit
git rebase -i HEAD~3          # Interactively rebase last 3 commits
git cherry-pick <commit>      # Apply specific commit
```
