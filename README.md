
# Setup 

git config --global user.name "<username>"
git config --global user.email "<email>"
git config --list

# Basic One

ls          // show all files
ls -a       // show all hidden files
git clone <--Link-->      // clone into your local pc
git status                // there are some common status
// Untracked = new files that git doesnt yet track
// Modified = changed
// Staged = file is ready to be commited
// Unmodified = unchanged

git add <--file name-->/.  // if we have more than 1 file to add we use .
git commit -m "Some message with this commit" 

#Push-upload local repo content to remote repo

git init
git remote add origin <--link-->
git remote -v  //to verify remote
git branch     //to check braanch
git branch -M main  //to rename the branch
git push origin main

//Note: If you are going to work on a project for long time , instead of writing "git push origin main" repeatativly , we can write "git push -u origin main" and then whenever we want to push , we just use "git push".

# Git Branches

git branch  //to check branch
git branch -M main  //to rename branch
git checkout <--branch name-->  //to navigate to some branch
git checkout -b <--new branch name-->  //create a new branch
git branch -d <--branch name-->  //delete a branch

# Merging Code

# way 1
git diff <--branch name-->  //to compare
git merge <--branch name-->  //to merge


# way 2
// by creating pull request (PR)

# Merge Conflicts

# Undoing Changes

# case 1  //Staged Changes
git reset <--file name-->
git rest

# case 2  //Commited Chnages ( for one commit)
git reset HEAD~1

# case 3 //Commited Changes (for many commits)
git reset <--commit hash-->
git reset --hard <--commit hash-->
