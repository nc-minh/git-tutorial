# Git Tutorial
Git is a version control system that allows you to track changes made to your code over time. This tutorial will guide you through some of the most commonly used Git commands.

## Installation
First, download Git from the official website: https://git-scm.com/downloads
To check if Git is installed on your machine, open a terminal and type:
```
git version
```

## Configuration
Before you start using Git, you need to configure your author information.
To set your name and email address:
```
git config --global user.name "Your Name"
git config --global user.email "Your Email"
```
You can also edit your author information after committing by using the command:
```
git commit --amend --reset-author
```

## Concept
There are three main areas in Git:
- Working directory: where you edit your files
- Staging area: where you stage changes to be committed
- Git repository: where committed changes are stored
To show a list of remote repositories, use the command:
```
git remote -v
```
## Basic Syntax
### Check status of folder
To check the status of your repository, use the command:
```
git status
```
### Create a repository
To create a new repository in your current directory, use the command:
```
git init
```
### Add files
To add a new file to the staging area, use the command:
```
git add <file name>
```
To add all modified files to the staging area, use the command:
```
git add .
```
### Commit changes
To commit your changes, use the command:
```
git commit -m "message"
```
Alternatively, you can add and commit changes in one step using:
```
git commit -a -m "message"
```
### Modify commit message
If you need to modify the message of your most recent commit, use the command:
```
git commit --amend -m "new message"
```
### Push changes
To push your changes to a remote repository, use the command:
```
git push
```
If you need to push to a specific branch, use the command:
```
git push origin <branch name>
```

>>If you encounter an authentication error when pushing to GitHub, refer to these resources:
<a href="https://github.blog/2020-12-15-token-authentication-requirements-for-git-operations/">token-authentication-requirements</a>
<a href="https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token">creating-a-personal-access-token</a>

### View commit history
To view the commit history, use the command:
```
git log
```
To view the changes made in a specific commit, use the command:
```
git show <commit id>
```
### View modified files
To view the changes made to modified files, use the command:
```
git diff
```
### Clone a repository
To clone a repository from a remote server, use the command:
```
git clone <repository url>
```
### Pull changes
To pull changes from a remote repository, use the command:
```
git pull
```
If you need to merge unrelated histories, use the command:
```
git pull origin <branch name> --allow-unrelated-histories
```
### Review changes on GUI
To review the modifications made to your files on a GUI, use the command:
```
gitk
```
### Unstage files
To unstage a file from the staging area, use the command:
```
git reset HEAD <file>
```
### Git checkout file
To discard changes in a modified file:
```
git checkout -- <file>
```
### Git branch and checkout
To create a new branch and switch to it:
```
git checkout -b <branch name>
```
### Check branch
To list all local branches and show the current branch:
```
git branch
```
To create a new branch from an existing branch:
```
git branch <new branch> <existing branch>
```
### Git checkout
To switch to the master branch:
```
git checkout master
```
### Git merge
To merge branch B into branch A:
- Switch to branch A: git checkout A
- Merge branch B into A: git merge B
### Git delete branch
To delete a local branch:
```
git branch -D <branch name>
```
### Undo commits
To undo a commit by ID:
- `--soft`: Undo the commit and keep changes in staging area.
- `--mixed`: Undo the commit and keep changes in working directory.
- `--hard`: Undo the commit and delete changes.
```
git reset --soft <commit ID>
```
```
git reset --mixed <commit ID>
```
```
git reset --hard <commit ID>
```
### Git revert
To revert a commit:
```
git revert <commit ID>
```
### Create .gitignore
To create a .gitignore file that ignores certain files when committing:
```
<file name>
```
### Git fetch
To fetch changes from a remote branch without merging:
```
git fetch <remote> <branch>
```
### Git rebase
To rebase changes from one branch onto another:
```
git rebase <branch with conflicts>
```
### Git push --force
To overwrite the remote branch with local changes:
```
git push --force
```
Note: This is not recommended as it can cause conflicts with other collaborators.
### Git stash
To temporarily save changes and revert back to a clean working directory:

```
git stash
```
To retrieve the most recent stash:
```
git stash apply
```
To retrieve a specific stash by ID:
```
git stash apply <stash ID>
```
