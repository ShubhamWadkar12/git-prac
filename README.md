# Git practise
Learning Git
Working on feature branch
Login feature in progress
 ## DevOps Learning


## Currently learning DevOps and Platform Engineering:

- Linux
- Bash
- Git
- GitHub 


## Monitoring

Learning Prometheus and Grafana for infrastructure monitoring.


# Git Essential Commands for DevOps

| Command | Description |
|---|---|
| `git init` | Initialize a new Git repository. |
| `git clone <repo-url>` | Clone an existing repository. |
| `git status` | Check repository and working-tree status. |
| `git add <file>` | Stage a specific file. |
| `git add .` | Stage all changes. |
| `git commit -m "message"` | Create a commit with a message. |
| `git log --oneline` | View compact commit history. |
| `git diff` | View unstaged changes. |
| `git diff --staged` | View staged changes. |
| `git branch` | List local branches. |
| `git switch <branch>` | Switch to a branch. |
| `git switch -c <branch>` | Create and switch to a new branch. |
| `git merge <branch>` | Merge another branch into the current branch. |
| `git rebase <branch>` | Rebase current branch onto another branch. |
| `git rebase --continue` | Continue rebase after resolving a conflict. |
| `git rebase --abort` | Cancel an ongoing rebase. |
| `git reset --soft HEAD~1` | Undo commit but keep changes staged. |
| `git reset --mixed HEAD~1` | Undo commit but keep changes unstaged. |
| `git reset --hard HEAD` | Discard uncommitted changes. |
| `git revert <commit>` | Create a new commit that undoes an earlier commit. |
| `git stash` | Temporarily save uncommitted changes. |
| `git stash pop` | Restore the latest stashed changes. |
| `git stash list` | List saved stashes. |
| `git cherry-pick <commit>` | Apply a specific commit to the current branch. |
| `git remote -v` | View configured remote repositories. |
| `git fetch` | Download remote updates without changing the current branch. |
| `git fetch --prune` | Fetch updates and remove stale remote branches. |
| `git pull` | Fetch and integrate remote changes. |
| `git push` | Push commits to the configured remote branch. |
| `git push -u origin <branch>` | Push a branch and set its upstream tracking branch. |
| `git push origin --delete <branch>` | Delete a remote branch. |
| `git branch -a` | List local and remote-tracking branches. |
| `git branch -vv` | Show branch tracking and ahead/behind status. |
| `git tag -a v1.0.0 -m "Release"` | Create an annotated release tag. |
| `git push origin v1.0.0` | Push a tag to the remote repository. |
| `git show <commit>` | Inspect a commit and its changes. |
| `git blame <file>` | See which commit/author changed each line. |
| `git rm --cached <file>` | Stop tracking a file while keeping it locally. |
| `ssh -T git@github.com` | Test GitHub SSH authentication. |

## Essential Git Workflow

```bash
git switch master
git pull

git switch -c feature-name

# Make changes

git status
git diff

git add .
git commit -m "Add feature"

git push -u origin feature-name

# Create Pull Request → Review → Merge

git switch master
git pull

git branch -d feature-name
git fetch --prune
```

## Git Mental Model
```
Working Directory
       ↓ git add
Staging Area
       ↓ git commit
Local Repository
       ↓ git push
Remote Repository
```

## Most Important Commands to Remember
```
git status      → What's happening?
git diff        → What changed?
git add         → Stage changes
git commit      → Save changes
git switch      → Change branch
git merge       → Combine branches
git rebase      → Replay commits
git stash       → Temporarily save work
git revert      → Safely undo a commit
git fetch       → Get remote updates
git pull        → Get + integrate updates
git push        → Send changes to remote
```
