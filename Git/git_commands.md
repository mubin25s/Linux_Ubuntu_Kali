# Common Git Commands Reference

This guide provides a quick reference for essential Git commands used in version control.

## 1. Getting Started
| Command | Description |
| :--- | :--- |
| `git init` | Initialize a new local Git repository. |
| `git clone <url>` | Clone a repository from a remote source. |

## 2. Basic Snapshotting
| Command | Description |
| :--- | :--- |
| `git add <file>` | Add a specific file to the staging area. |
| `git add .` | Add all changed files to the staging area. |
| `git commit -m "message"` | Commit staged changes with a descriptive message. |
| `git status` | Show the status of your working directory and staging area. |
| `git log` | Show the commit history for the current branch. |
| `git log --oneline` | Show a condensed version of the commit history. |
| `git diff` | Show changes between working directory and staging area. |

## 3. Branching and Merging
| Command | Description |
| :--- | :--- |
| `git branch` | List all local branches. |
| `git branch <name>` | Create a new branch. |
| `git checkout <branch>` | Switch to a different branch. |
| `git checkout -b <name>` | Create and switch to a new branch. |
| `git switch <branch>` | Modern way to switch branches. |
| `git merge <branch>` | Merge the specified branch into the current branch. |
| `git branch -d <name>` | Delete a local branch. |

## 4. Remote Repositories
| Command | Description |
| :--- | :--- |
| `git remote add origin <url>` | Connect a local repository to a remote server. |
| `git push -u origin <branch>` | Push changes to the remote repository and set upstream. |
| `git push` | Push committed changes to the remote repository. |
| `git pull` | Fetch and merge changes from the remote repository. |
| `git fetch` | Download changes from the remote repository without merging. |

## 5. Undoing Changes
| Command | Description |
| :--- | :--- |
| `git restore <file>` | Discard changes in the working directory. |
| `git reset HEAD <file>` | Unstage a file while keeping changes. |
| `git reset --soft HEAD~1` | Undo the last commit, keeping changes in the staging area. |
| `git reset --hard HEAD~1` | Undo the last commit and discard all changes. |
| `git revert <commit-id>` | Create a new commit that undoes the changes of a specific commit. |

## 6. Stashing
| Command | Description |
| :--- | :--- |
| `git stash` | Temporarily store all modified tracked files. |
| `git stash pop` | Restore the most recently stashed changes. |
| `git stash list` | List all stashed changes. |

## 7. Configuration
| Command | Description |
| :--- | :--- |
| `git config --global user.name "Your Name"` | Set your global username. |
| `git config --global user.email "email@example.com"` | Set your global email address. |
| `git config --list` | List all Git configurations. |
