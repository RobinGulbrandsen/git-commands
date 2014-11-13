# Info

Open repository with cheat cheep git commands. This document will be updated with new commands as the need presents themselves

# Commands

**Initiate git for the directory**
    git init

**Add file to git version control**
    git add [filename]
    git add [foldername]
    git add .

**Commit files with message on "m" flag**
    git commit -m "[message]"

**Add which remote location code should be commited to**
    git remote add [name of the repository] [git repository]
    git remote add origin https://github.com/RobinGulbrandsen/git-commands.git

**Push til git repo**
    git push -u [name of the repository] [branch]
    git push -u origin master

**Clone repository from GitHub to local machine**
    git clone [source]

**Get code updates from repository**
    git pull [source]

**Check status on files in the direcotry**
    git status

**Create new branch (copys all elements in your current branch)**
    git checkout -b [name]
    git checkout -b new-dev-branch

**Create new empty branch
    git checkout --orpahn [name]

Now you have a branch with all the files, but no commit. So remove the files

    git rm -rf .

Now you got a new branch with no files in it.

**Copy files or folders from one branch to an other**

1. Swtich to the branch you want the files to be copied to

    git checkout new-dev-branch

2. Get the files or folders you want to copy over

    git checkout [branch to be copied from] -- [file or folder]
    git checkout master -- src/

**Rollback all changes that has not been commited**
    git checkout .

**Rolback changes from file or folder that has not been commited**
    git checkout [file or folder]
