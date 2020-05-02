# Everything you need to know for Git

I am writing this for not an absolute solution to most of the issues but to help in remembering git commands. I am uploading this to [Github](https://github.com/mkumail1) so that I can comeback and check the things for myself later on.

## Getting Started

For me these commands are the most important and are basically a crash cheat sheet for most of the common commands used in git. If executed perfectly you won't be needing any other command for work.

### 1. Initializing a git repository in your current folder

```
git init
```

### 2. Creating a *new file*

```
touch <filename>
```

### 3. Opening a file using a text editor such as *atom*

```
atom <filename>
```

### 4. Changing *name* of a file

```
mv <previousname> <newname>
```

## Bread and Butter of git

### a. *Adding* files to the repository

```
git add <filename> <filename> 
```
or use a '.' to add all of the files in a folder 

or use ‘*’ to add file of a certain type such as  * *.html* will add all .html files in a directory

### b. *Commiting* changes

```
git commit -m "message"
```
-m is used for not opening a commit file in CLI

### 5. Checking *status*

```
git status
```
git **tracked** files means they are added and read by git

**untracked** files means that they are not added or catered by git

### 6. *Removing* a file from commit

```
git rm --cached <filename>
```

### 7. Removing a file from the *main* directory
```
rm <filename>
```

### 8. Checking git *commit's* history

```
git log
```

### 9. Visiting back to a *commit*

```
git checkout <commit code>
```

### 10. Reverting/walking back to a *commit* from *master* branch 

```
git revert --no-commit <commit code>..HEAD
```
Note: you will still have the history of recent updates even if you go back

### 11. Creating a *.gitignore* file

```
touch .gitignore
```
used for ignoring some git files
just add names of files inside this *.gitignore* file and they will vanish

### 12. For adding a *.gitignore* file in commit

```
git add -A
```
This will add every file including *.gitignore* for next commit

### 13. For creating a *new branch*

```
git checkout -b <branchname> or git branch <branchname>
```

### 14. For *deleting* a branch

```
git branch -d <branchname>
```

### 15. Check *list* of branches

```
git branch
```

### 16. *Moving* to any branch

```
git checkout <branchname>
```

### 17. For merging a *branch*

```
git merge <branch_name_other_than_master>
```
This will automatically create a commit to git as well
If you want to merge into *master* branch -> make sure you are currently in *master* branch 

### 18. Adding a remote link <*branch*> of a repositiory

```
git remote add origin master
```
**Remote:** here is the remote origin

**Add:** means we are adding something to a remote rep

**Origin:** is a name for the push, can be anything else

**Master:** is a <*branch name*>, can be any other branch as well

### 19. Adding a remote link <*url*> of a repositiory

```
git remote add origin <url>
```
**Remote:** here is the remote origin

**Add:** means we are adding something to a remote rep

**Origin:** is a name for the push, can be anything else

**url:** is the url of the reporsitory you want to add to your git bash

Note: For existing repositories first check *git pull* for checking the current status and then commit changes.

### 20. Pushing everything to the remote repository

```
git push -u origin master
```

## 21. For making a pull request

1. Go to any github repository [for example](https://github.com/mkumail1/PurrfectMatchingHTML-CSS).
2. Tap on folk.
3. Copy the link of the repository.
4. Open terminal and type.
```
git clone <url>
```
4. Make changes, then commit.
5. Afterwards use [pull request](https://github.com/mkumail1/PurrfectMatchingHTML-CSS/pulls) to make a request.

## Acknowledgments

Muhammad Kumail 

[Github](https://github.com/mkumail1)

[Linkedin](https://www.linkedin.com/in/mkumail1/)

[Twitter](https://www.twitter.com/thezwitterguy)

[Facebook](https://www.facebook.com/thezwitterguy)

