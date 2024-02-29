# Starting my Git timeline

## Initialise your Git by using `git init`

```Go
cd /Users/sohyungkim/Desktop/Workspace/VIB_Training/Github
```

When writing a commit, you have to include why was it changed, how this addresses the issue, and the effects due to the change. Most importantly, you should mention limitation of the change, meaning that you should mention if your changes are complete or not. Be as descriptive as possible!!!



## 1. Make a file in your working directory (developmental area) locally with MarkText.



## 2. Add the local file into the staging area.

```
git add [filename.md]
```

## 

## 3. Saving a timepoint by using `git commit -m [message]`

```
# Saves the update version (snapshot/point in time) in git repo
git commit -m "meaningful msg"
```







# Git status

It will check all 3 conceptual areas to see if the files are **unstaged/changes to be comitted/untracked***. Then, you can make a decision of what to do with the files in the **staging area**. Here, than you can use `git commit` to submit to the **local repository**.

```
git status

# Changes to be committed: in the staging area
# Changes not staged: modified, but did not got added to the staging area
# Untracked files: file that has never been added/committed
```




