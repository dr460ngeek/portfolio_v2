# Git Cheatsheet (Enhanced)

## Setup & Configuration
| Command | Action |
|---------|--------|
| ```git config --global user.name "Your Name"``` | Set global username |
| ```git config --global user.email "you@example.com"``` | Set global email |
| ```git config --list``` | Show all Git config settings |
| ```git help <command>``` | Show help for a Git command |

---

## Repository Management
| Command | Action |
|---------|--------|
| ```git init``` | Initialize a new Git repository |
| ```git clone <url>``` | Clone repository from URL |
| ```git status``` | Show status of working directory and staging area |
| ```git log``` | Show commit history |
| ```git log --oneline --graph --all``` | Compact history with branches |
| ```git show <commit>``` | Show details of a commit |

---

## Staging & Committing
| Command | Action |
|---------|--------|
| ```git add <file>``` | Stage file for commit |
| ```git add .``` | Stage all changes in current directory |
| ```git reset <file>``` | Unstage a file (keep changes) |
| ```git commit -m "message"``` | Commit staged changes with message |
| ```git commit -am "message"``` | Stage and commit tracked files in one step |
| ```git diff``` | Show changes in working directory |
| ```git diff --staged``` | Show changes staged for next commit |

---

## Branching & Merging
| Command | Action |
|---------|--------|
| ```git branch``` | List local branches |
| ```git branch <name>``` | Create a new branch |
| ```git checkout <branch>``` | Switch to branch |
| ```git switch <branch>``` | Switch branch (newer command) |
| ```git switch -c <branch>``` | Create and switch to new branch |
| ```git merge <branch>``` | Merge given branch into current |
| ```git branch -d <branch>``` | Delete branch (safe) |
| ```git branch -D <branch>``` | Force delete branch |

---

## Remote Repositories
| Command | Action |
|---------|--------|
| ```git remote -v``` | Show remotes |
| ```git remote add origin <url>``` | Add new remote |
| ```git fetch origin``` | Download objects/refs from remote |
| ```git pull origin main``` | Fetch and merge remote branch into local |
| ```git push origin main``` | Push local branch to remote |
| ```git push -u origin <branch>```| Push and set upstream branch |
| ```git remote remove <name>```| Remove remote |

---

## Undoing Changes
| Command | Action |
|---------|--------|
| ```git restore <file>``` | Discard changes in working directory |
| ```git restore --staged <file>``` | Unstage file (newer command) |
| ```git reset HEAD <file>``` | Unstage file (older syntax) |
| ```git reset --soft HEAD~1``` | Undo last commit, keep changes staged |
| ```git reset --mixed HEAD~1``` | Undo last commit, keep changes in working directory |
| ```git reset --hard HEAD~1``` | Undo last commit and discard changes |
| ```git revert <commit>``` | Create new commit that reverts given commit |

---

## Stashing
| Command | Action |
|---------|--------|
| ```git stash``` | Save uncommitted changes temporarily |
| ```git stash save "msg"``` | Stash with description |
| ```git stash list``` | List stashes |
| ```git stash pop``` | Apply last stash and remove it |
| ```git stash apply``` | Apply last stash (keep in stash list) |
| ```git stash drop``` | Remove last stash |
| ```git stash clear``` | Remove all stashes |

---

## Tagging
| Command | Action |
|---------|--------|
| ```git tag``` | List tags |
| ```git tag <name>``` | Create lightweight tag |
| ```git tag -a <name> -m "message"``` | Create annotated tag |
| ```git show <tag>``` | Show tag details |
| ```git push origin <tag>``` | Push tag to remote |
| ```git push origin --tags``` | Push all tags |

---

## Inspection & Shortcuts
| Command | Action |
|---------|--------|
| ```git log -p```| Show commits with diffs |
| ```git log --stat``` | Show commit history with file stats |
| ```git blame <file>``` | Show who last modified each line |
| ```git shortlog -sn``` | Show commit count per contributor |
| ```git reflog``` | Show history of HEAD changes |
| ```git gc``` | Cleanup unnecessary files and optimize repo |

