# The Engineer’s Corner - GIT CheatSheet

Author: &nbsp; William FitzPatrick  
Date:&nbsp;  &nbsp; &nbsp; Aug 04 2022  
Version: 1.017  

## Introduction

I list below many of the most common commands in GIT  
To maximize effectiveness of the list below, I recommend you add them to your gitconfig aliases

---

## Create and Clone

| Command                                                         | Desc                                                                  |
|-----------------------------------------------------------------|-----------------------------------------------------------------------|
| git init                                                        | Initialize a local Git repository                                     |
| git clone repo_url                                              | Clone public repository                                               |

## Add and Remove

| Command                                                         | Desc                                                                  |
|-----------------------------------------------------------------|-----------------------------------------------------------------------|
| git add [file-name]                                             | Add a file to the staging area                                        |
| git add -A                                                      | Add all new and changed files to the staging area                     |
| git rm -r [file-name.txt]                                       | Remove a file (or folder)                                             |
| git commit -m "[commit message]"                                | Commit changes             

## Audit and Analyze                                          

| Command                                                         | Desc                                                                  |
|-----------------------------------------------------------------|-----------------------------------------------------------------------|
| git status                                                      | Check status                                                          |
| git status -sbu                                                 | Check status with concise, branch info, and untracked file details    |
| git log                                                         | View changes                                                          |
| git log --summary                                               | View changes (detailed)                                               |
| git log --oneline                                               | View changes (briefly)                                                |
| git diff [source branch] [target branch]                        | Preview changes before merging                                        |

## Undo and Restore  

| Command                                                         | Desc                                                                  |
|-----------------------------------------------------------------|-----------------------------------------------------------------------|
| git revert commitid                                             | Revert commit changes                                                 |

## Synchronize

| Command                                                         | Desc                                                                  |
|-----------------------------------------------------------------|-----------------------------------------------------------------------|
| git fetch origin [branch name]                                  | Download commits, files, and refs from a remote repository into your local repo |	    
| git pull                                                        | Update local repository to the newest commit                          |
| git pull origin [branch name]                                   | Pull changes from remote repository                                   |
| git push origin --delete [branch name]                          | Delete a remote branch                                                |
| git push origin [branch name]                                   | Push a branch to your remote repository                               |
| git push -u origin [branch name]                                | Push changes to remote repository (and remember the branch)           |
| git push                                                        | Push changes to remote repository (remembered branch)                 |
| git push origin --delete [branch name]                          | Delete a remote branch                                                |
| git stash                                                       | Stash changes in a dirty working directory                            |
| git stash clear                                                 | Remove all stashed entries                                            |

## Branch

| Command                                                         | Desc                                                                  |
|-----------------------------------------------------------------|-----------------------------------------------------------------------|
| git branch                                                      | List of branches (the asterisk denotes the current branch)            |
| git branch -a                                                   | List all branches (local and remote)                                  |
| git branch [branch name]                                        | Create a new branch                                                   |
| git branch -d [branch name]                                     | Delete a branch                                                       |
| git branch -D [branch name]                                     | Delete a branch forcefully                                            |
| git checkout -b [branch name]                                   | Create a new branch and switch to it                                  |
| git checkout -b [branch name] origin/[branch name]              | Clone a remote branch and switch to it                                |
| git branch -m [old branch name] [new branch name]               | Rename a local branch                                                 |
| git checkout [branch name]                                      | Switch to a branch                                                    |
| git checkout -                                                  | Switch to the branch last checked out                                 |
| git checkout -- [file-name.txt]                                 | Discard changes to a file                                             |

## Merge

| Command                                                         | Desc                                                                  |
|-----------------------------------------------------------------|-----------------------------------------------------------------------|
| git merge [branch name]                                         | Merge a branch into the active branch                                 |
| git merge [source branch] [target branch]                       | Merge a branch into a target branch                                   |
| git rebase origin/master --ff-only                              | Merge a pending changes in origin master into your local master                                   |


## Remote

| Command                                                         | Desc                                                                  |
|-----------------------------------------------------------------|-----------------------------------------------------------------------|
| git remote add origin [url]                                     | Add a remote repository                                               |
| git remote set-url origin [url]                                 | Set a repository's origin branch to SSH                               |

## Configure

| Command                                                         | Desc                                                                  |
|-----------------------------------------------------------------|-----------------------------------------------------------------------|
| git config --global user.name "your_username"                   | Set globally Username                                                 |
| git config --global user.email "sample@gmail.com"               | Set globally Email id                                                 |
| git config --global --list                                      | Get global config                                                     |

---

## References

[Git Commands - LoginRadius](https://www.loginradius.com/blog/engineering/git-commands)
