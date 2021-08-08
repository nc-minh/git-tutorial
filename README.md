# Tutorial-git 

<a href="https://git-scm.com/downloads">Download Git</a>

<h3>Check version</h3>

```
git version
```
<h3>Save author</h3>

```
Git config --global user.name = “Your Name”
```
```
Git config --global user.email = “Your Mail”
```
```
Git config --global user.password = “Your Password”
```
## Concept
```
- Working directory
- Staging area
- Git Repository
```
## Syntax
### Check status folder
```
git status
```

### Create a repository in your pc
```
git init
```

### Add new file
```
git add "file name"
```
or
```
git add .
```

### Add commit
```
git commit -m"message"
```
or(add and commit)
```
git commit -a -m"message" 
```
### Git push
```
git push
```
### Git log
Review commit history
```
git log
```
### Git show 
Show commit history and content
```
git show + (id commit)
```
### Git diff 
Review the contents of the 'modified' file
```
git diff
```
### Git clone
```
git clone
```
### Gitk
Review the modifications on the GUI
```
gitk
```
### Git reset
Unstage 'modified' file
```
git reset HEAD <file>
```
### Git checkout file
Delete 'modified' file
```
git checkout -- <file>
```
### Git branch and checkout
Create new branch
```
git checkout -b <branch name>
```
<img src="img/git.JPG" alt="github">
<img src="img/tutorial github.JPG" alt="github">
