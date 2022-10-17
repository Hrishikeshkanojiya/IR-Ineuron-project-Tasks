# Assignment 1 Answers:
---
<img src="https://user-images.githubusercontent.com/43959475/193852439-ecf91e2d-c234-40d6-9639-10302efd9ab5.gif" width="30%" height="30%"/>

---
## Task 1:  ( 15 Basic Git Commands ):

###  1) git version :
Git is a version control system that developers use all over the world. It helps you track different versions of your code and collaborate with other developers.</br>
If you are working on a project over time, you may want to keep track of which changes were made, by whom, and when those changes were made.
```bash
git --version
```
![Git-version](https://user-images.githubusercontent.com/96219205/195533532-5c57d37a-7ba2-4e13-92b9-97ffe038d2dd.png)

### 2) git init :
The git init command creates a new Git repository. It can be used to convert an existing, unversioned project to a Git repository or initialize a new,</br>
empty repository. Most other Git commands are not available outside of an initialized repository, so this is usually the first command you'll run in a new project.
```bash
git init
```
![Git-Init](https://user-images.githubusercontent.com/96219205/195777043-208a3aa7-6435-4d68-8d2e-5aed9f4de2a1.png)
### 3) git config :
This command sets the author name and email address respectively to be used with your commits.
```
git config --global user.name "USER NAME"
git config --global user.email "USEREMAIL@gmail.com"
```
![Git config](https://user-images.githubusercontent.com/96219205/196125385-850141f7-378e-407c-b840-7c85d5ccfba5.png)

### 4) git status :
This command will show the modified status of an existing file and the file addition status of a new file, if any, that has to be committed.
```bash
git status
```
![Git-status](https://user-images.githubusercontent.com/96219205/195777197-71137216-033c-4781-81ba-c66b29c095a3.png)
### 5) git add :
This command adds one or more to the staging area.
```bash
git add .
```
![Git-add](https://user-images.githubusercontent.com/96219205/195777335-c88f016d-a475-4858-8043-9afbca7703cf.png)
### 6) git remote :
Once everything is ready on our local system, we can start pushing our code to the remote (central) repository of the project. </br>
Click on the Copy icon on the right side of the URL box of the Github repository to copy the link and paste it as shown below:</br>
git remote add origin “URL” </br>
Now, we are ready to operate the remote commands in our repository that we have just created.
```bash
git remote -v
```
![Git-remote](https://user-images.githubusercontent.com/96219205/195777437-3a4c8686-d9c3-46f2-885e-3a4fc4bb0f2f.png)

### 7) git commit :
This command commits any files you’ve added with the git add command and also commits any files you’ve changed since then.
```bash
git commit -m "this is an commit massage"
```
![git commit](https://user-images.githubusercontent.com/96219205/195779961-92f787a6-b5dc-4196-a073-77bbdf3e5ac8.png)

### 8) git push :
Suppose, we have made some changes in the file and want to push the changes to our remote repository on a particular branch. By using the command ‘git push,’</br>
the local repository’s files can be synced with the remote repository on Github.
```bash
git push -u origin main 
```
![git push](https://user-images.githubusercontent.com/96219205/195785478-1e123f3d-06d7-4635-acc6-d41a6f01c105.png)

### 9) git branch :
Suppose, we have made some changes in the file and want to push the changes to our remote repository on a particular branch.</br> 
By using the command ‘git push,’ the local repository’s files can be synced with the remote repository on Github.

```bash
git branch -a
```
![git branch](https://user-images.githubusercontent.com/96219205/195787427-f177e9c9-4045-4d4d-8ef5-cbc9ea67f83f.png)

Similarly, to delete a branch, we use the **git branch -D command:**
  
```bash
git branch -D 
```
![git branch -d](https://user-images.githubusercontent.com/96219205/196125224-68162e8f-f63c-4616-9a6b-c3273a984aaa.png)

### 10) git checkout:
We use this command to navigate to an existing branch, add new files, and commit the files:
```bash
git checkout devloper1
```
![git checkout](https://user-images.githubusercontent.com/96219205/196123908-9610c1a8-4946-480a-9f8a-626158428abd.png)

We use this command to create a branch and navigate to that particular branch (say, the ‘name-of-the-new-branch’ is ‘branch2’) at the same time:
```bash
git checkout -b devloper1
```

![git checkout -b](https://user-images.githubusercontent.com/96219205/196124083-222cbb95-1e91-4d4b-a80f-41f96322a5a2.png)

### 11) git merge:
Merging is Git's way of putting a forked history back together again. The git merge command lets you take the independent lines of development </br>
created by git branch and integrate them into a single branch. Note that all of the commands presented below merge into the current branch.
```bash
git merge devloper1
```
![GIT MERGE](https://user-images.githubusercontent.com/96219205/196124435-b7b3abb6-a555-4dac-a925-e604ff112a7b.png)

### 12) git log:
Th is command is used when we want to check the log for every commit in detail in our repository.
```bash
git log
```
![git log](https://user-images.githubusercontent.com/96219205/196124513-3d81dd05-40d1-437c-bc41-90ae8c47ce57.png)

### 13) git stash:
git stash temporarily shelves (or stashes) changes you've made to your working copy so you can work on something else,</br>
and then come back and re-apply them later on
```bash
git stash
```
![git stash](https://user-images.githubusercontent.com/96219205/196124631-99625009-e87c-4d6e-9bfa-a5f97b6b219e.png)

### 14) git revert:
The git revert command can be considered as an ‘undo’ command. However, it does not work as the traditional ‘undo’ operation.</br>
It figures out how to invert the changes introduced by the commit and appends a new commit with the resulting inverse content.

```bash
git revert [commit id]
```

![git revert](https://user-images.githubusercontent.com/96219205/196124763-4847bb99-0187-4cb4-a689-045108f0daf7.png)

### 15) git rebase: 
Rebase is the process of moving and combining a sequence of commits to a new base commit. Rebasing is changing </br>
the base of our branch from one commit to another, making it appear as if we’ve created our branch from a different commit.</br>
Internally, Git accomplishes this by creating new commits and applying them to the specified base. It’s very important to understand </br>
that even though the branch looks the same, it is composed of entirely new commits. The git rebase command performs an automatic </br>
git checkout <branch> before doing anything else.Otherwise, it remains on the current branch.

```bash
git rebase main
```
![git rebase](https://user-images.githubusercontent.com/96219205/196124865-df2eb8a0-0b01-423b-8b1c-769733de94b3.png)

### 16) git fetch:
When we use the command git fetch, Git gathers any commit from the target branch that does not exist in our current</br>
branch and stores it in our local repository. However, it does not merge it with our current branch.

```bash
git fetch --all
```
![git fetch ](https://user-images.githubusercontent.com/96219205/196125070-03bb9e2c-bc5e-4940-ba9f-39d44ae50192.png)

