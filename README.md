# Everything you need to know for Git

I am writing this for not an absolute solution to most of the issues but to help in remembering git commands. I am uploading this to gitHub so that I can comeback and check the things for myself later on.

## Getting Started

For me these commands are the most important and are basically a crash cheat sheet for most of the common commands used in git. If executed perfectly you won't be needing any other command for work.

### Initializing a git repository in your current folder

```
git init
```

### Creating a new file

```
touch <filename>
```

### Opening it using a text editor such as atom

```
atom <filename>
```

### Changing name of a file

```
mv <previousname> <newname>
```

## Bread and Butter of git

### 1. Adding files to the repository

```
git add <filename> <filename> 
```
or use a '.' to add all of the files in a folder 

or use ‘*’ to add file of a certain type such as  * *.html* will add all .html files in a directory

### 2. Commiting changes

```
git commit -m "message"
```
-m is used for not opening a commit file in CLI

### Checking status

```
git status
```
git **tracked** files means they are added and read by git

**untracked** files means that they are not added or catered by git

### Removing a file from commit

```
git rm --cached <filename>
```

### Removing a file from the main directory
```
rm <filename>
```

### Checking git commit's history

```
git log
```

### Visiting back to a commit

```
git checkout <commit code>
```

### Reverting/walking back to a commit from master branch 

```
git revert --no-commit <commit code>..HEAD
```
Note: you will still have the history of recent updates even if you go back

### Creating a *.gitignore* file

```
touch .gitignore
```
used for ignoring some git files
just add names of files inside this ‘.gitignore’ file and they will vanish

### For adding a .gitignore file in commit

```
git add -A
```
This will add every file including ***.gitignore*** for further commit

### For creating a new branch

```
git checkout -b <branchname> or git branch <branchname>
```

### For deleting a branch

```
git branch -d <branchname>
```

### Check list of branches

```
git branch
```

### Moving to any branch

```
git checkout <branchname>
```

### For merging a branch

```
git merge <branch_name_other_than_master>
```
This will automatically create a commit to git as well
If you want to merge into master -> make sure you are currently in master branch 

### Adding a remote link *<url>* of a repositiory

```
git remote add origin master
```
**Remote:** here is the remote origin
**Add:** means we are adding something to a remote rep
**Origin:** is a name can be anything else
**Master:** is a <branch name>, can be any other branch as well

### Pushing everything to the remote repository

```
git push -u origin master:
```

## For making a pull request

1. Go to folk
```
2. git clone <url>
```
3. Make changes then commit and afterwards use pull request to make a request.

## Acknowledgments

Muhammad Kumail - [mkumail1](https://github.com/mkumail1)
Linkedin - [mkumail1](https://www.linkedin.com/in/mkumail1/)
Twitter - [mkumail1](https://www.twitter.com/mkumail)

