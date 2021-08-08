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
### Check branch
Check current branch 
```
git branch
```
### Git checkout
Switch to branch 'master' 
```
git checkout
```
### Git merge
Branch merge 
if you want B --> A
first you have to 'checkout A'
then:
```
git merge B
```
### Git delete branch
Delete branch 
```
git branch -D <branch name>
```
### Git reset
Undo commit by id,
<p>--soft: return to the state before commit</p>
<p>--mixed: return to the state before add</p>
<p>--hard: delete previous commits </p>

```
git reset --soft <id_commit>
```
```
git reset --mixed <id_commit>
```
```
git reset --hard <id_commit>
```
### Git revert
Return commit
```
git revert <id_commit>
```
### Create .gitignore
Ignore the file you don't want to commit
```
<file name>
```
<img src="img/git.JPG" alt="github">
<img src="img/tutorial github.JPG" alt="github">
