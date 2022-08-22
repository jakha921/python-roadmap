# GitHub main commands

## Содержание:

1. [create a new repository and push it to GitHub](#create-new-repository-and-push-it-to-GitHub)
2. [connect to GitHub](#connect-to-GitHub)
3. [clone repository](#clone-repository)
4. [get all updates from GitHub](#get-all-updates-from-GitHub)
5. [create new branch](#create-new-branch)
6. [delete branch](#delete-branch)
7. [fetch branch](#fetch-branch)
8. [delete repository](#delete-repository)
9. [change remote repo to new ](#change-remote-repo-to-new )

# create new repository and push it to GitHub

    git init
    git add . / -A / --all (add all files)
    git commit -m "first commit"
    git remote add origin "link to repository"
    git push -u origin master

---

# connect to GitHub

    git remote add origin "link to repository"
    git push -u origin master

---

# clone repository

    git clone "link to repository"

---

# get all updates from GitHub

    git pull

---

# create new branch

    git checkout -b "new branch"
    git push -u origin "new branch"

---

# delete branch

    git branch -d "new branch"
    git push origin --delete "new branch"

--- 

# fetch branch

    git fetch origin "new branch"
    git checkout "new branch"
    git merge "origin/new branch"
    git push origin "new branch"

---

# delete repository

    git remote rm origin
    git rm --cached -r .
    git commit -m "delete repository"
    git push origin --delete

---

# change remote repo to new

    git remote set-url origin new.git.url/here

[//]: # (# cancel initial commit)

[//]: # (    git reset --hard HEAD~1)

[//]: # (    git push origin --force)




