# Some Basic Git and Github Commands

## Git Common Commands

### git init
- to initialize git for a specific folder we need to go into the folder and initialize the git so it can monitor the changes in it. It initializes an empty repository

### git status
- to see that status of our initialized repository. what files we have in our folder. which branch we are on, what is the status of untracked files , what we need to commit etc. give the information of current state of git repository

### git add filename or git add .
- "git add filename" adds a specific file to a stage. A stage is a step between tracked and untracked files. After we initialize a folder using git init git detects if any files are inside the directory. if we delete them before adding them git can't restore them. but if we add them and commit them then we can restore those files. "git add filename" adds a single file "git add ." add all the files inside our directory which can be risky if we want some files not to be tracked. git add actually adds the untracked files to a stage and once we commit we can track them properly. only adding them makes file recognizeable but not trackable. after commiting the files becomes trackeable.


### git commit - m "Message"
- to commit any changes to our repo. if we have made some changes to our files and we have added them we can use commit to permanently monitor those changes.

### git push -u origin master 
- to push code to a master branch. by default a master branch is initialized and created but we can create other branches tool.


## Git Branch Commands

### git checkout -b branchanme  or git branch new_branch_name
- to create a new branch with a specific branchname. it means to checkout from main/master branch and create a new branch.

### git checkout master
- to return to master branch from any other branch.

### git switch branchname
- to switch from one branch to another

### git ls-files
- to see which files are in a current branch

### git branch or git branch -av
- It list all the branches in our repo and also shows on which branch we are in with a * before our branch.

### git branch -d branchname
- to remove/delete a branch with specific branch name on our local repo.

### git push origin --delete branchname
- after deleting a branch from local repo we can reflect the changes in our remote server(github) by using above commands. this will delete the branch on github too.

### git merge branch_name 
- merges the current current content in branch_name to the current branch you are in .


## Git Diff Command

### git diff filename
- shows the difference between past content in the file and current file if you have removed any lines or add new ones.

### git diff branchname 
- Shows the difference in files between current branch you are in and the branch you mentioned



## Git Restore Commands

### git restore filename 
- to restore a deleted file

### git restore --staged filename
- to remove file after stagging using git add..

### git log
- to see the logs of git. what commits you made what changes you have done so on.

### git revert hashcode
- to revert back to a previous commit. hashcode can be obtained by using git log command which will show commits with a code.


## GitHub Commands to link with local git

### git pull "Repository_link"
- to pull any file created in github and we want it onto our local system

### git clone "Repository_link"
- to copy a repository created in gihub and we want to clone it into our local system git clone is used

### git remote add origin "link"
- to connect our local repo to remote (Github, Gitlaab , Bitbucket)

### git remote -v 
- to show any remote repositories connect to our local repo

### git push -u origin new_branch_here 
- to push code to a new branch



## Git Configure Commands

### git config --global user.name "Name" 
- to configure git globally

### git config --global user.email "Email"
- to configure git globally

### git config --list
- to see the list of globally configured git users on this computer

### git config --help 0r git help config
- to know information about any commands here only config is used
