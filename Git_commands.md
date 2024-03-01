Bruna Piereck

# Starting my Git timeline

## Initialise your Git by using `git init`

```Go
cd /Users/sohyungkim/Desktop/Workspace/VIB_Training/Github
```

When writing a commit, you have to include why was it changed, how this addresses the issue, and the effects due to the change. Most importantly, you should mention limitation of the change, meaning that you should mention if your changes are complete or not. Be as descriptive as possible!!!

## 1. Make a file in your working directory (developmental area) locally with MarkText.

## 2. Add the local file into the staging area by  `git add`

```
git add [filename.md]

git add * #to add all the files in the working directory 
```

## 3. Saving a timepoint by using `git commit -m [message]`

```
# Saves the update version (snapshot/point in time) in git repo
git commit -m "meaningful msg"
```

If you forget to put `-m` in `git commit`, then git will open you a **vi editor** to enter your message because he will NOT let you commit without any messages!

# Check git status by using `git status`

It will check all 3 conceptual areas to see if the files are **unstaged/changes to be comitted/untracked***. Then, you can make a decision of what to do with the files in the **staging area**. Here, than you can use `git commit` to submit to the **local repository**.

```
git status

# Changes to be committed: in the staging area
# Changes not staged: modified, but did not got added to the staging area
# Untracked files: file that has never been added/committed
```

# View history by using `git log`

This command will give you a **unique identifier** of each commit that you can access.

```bash
**>> sohyungkim@w235h175 Github % git log**
commit 95344a2353d5cc8a3a73ba46fa687485e0f7e91e (HEAD -> master)    #unique identifier
Author: sokim <sohyung.bella.kim@gmail.com>                         #author information
Date:   Thu Feb 29 13:33:13 2024 +0100                              #

    clarifying how to check where my files are in which conceptual areas and learned how to put all files to the staging area by using REGEX

commit be27d10d028009c5db055a9fcfa84639b7774388
Author: sokim <sohyung.bella.kim@gmail.com>
Date:   Thu Feb 29 13:15:24 2024 +0100

    splitting files into two for easy access to cheatsheet with concepts

commit 4a3b2a0149b4b5da9907aa9b8654a0040271f796
Author: So Hyung Kim <sohyungkim@MacBook-Pro-2.local>
Date:   Thu Feb 29 11:55:23 2024 +0100

    added info about 3 conceptual areas

commit cf61891c248419c8e8f92b7be4291f7b7ff429ec
Author: So Hyung Kim <sohyungkim@MacBook-Pro-2.local>
Date:   Thu Feb 29 11:39:55 2024 +0100

    brief description of differences between git and Github and how to get started with gi
```

### Set your own unique identifier by using `git log --help`

```bash
git log -n 5              #show 5 recent commits
git log --abbrev-commit   #gives short version of the unique identifier
```

# Travel back in time

Like any other time travel movies, be careful making changes in the past that might have consequence in the future!

```bash
# shows the commits you asked for comparison
git show <commit ID 1> <commit ID 2>
```

```bash
# shows the **difference** between the two commits in a **line-by-line comparison**
git diff <commit ID 1> <commit ID 2>
```



```
git revert HEAD~1
```
