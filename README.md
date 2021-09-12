# git
## Introduction
* What is git?
  * A kind of distributed version control system
* Why git?
  * Track history
  * Work together
* Three different levels of user
  * System: all users
  * Global: all repositories of the current user
  * Local: the current repository
* Structure of git  
  <img width="350" alt="截圖 2021-09-07 下午4 16 51" src="https://user-images.githubusercontent.com/61928785/132310006-462848e4-ec04-49f9-a800-c57b280ad673.png">
## Basic commands
* check the version of git
  ```
  git --version
  ```
* Setting
  ```
  git config --global user.name "<your name of account>"
  git config --global user.email <your email>
  ```
* Clone repo
  ```
  git clone <URL>
  ```
* Push repo
  * You will need to input your username and passward after `git push`, but the passward here is not your Github's passward. First of all, you have to go to **Settings** => **Developer Settings** => **Personal Access Token** => Fillup the form => click **Generate Token** and then copy it for the passward.  
  ```
  # start a new repo locally
  git init
  # add a remote repo
  git remote origin add <URL>
  # add a change in the working directory to the staging area
  git add <your file>
  # Take the staged snapshot and commits it to the project history
  git commit -m "<description>"
  # push to your repo on Github
  git push
  ```
* Check file ststus
  ```
  git status
  ```
* Use git to delete a file
  ```
  git rm <file>
  # update all files status
  git add -u
  git commit -m "<Remove a file>"
  # find out the history
  git log
  ```
## Reference
* <https://www.youtube.com/watch?v=8JJ101D3knE>
* <https://blog.techbridge.cc/2018/01/17/learning-programming-and-coding-with-python-git-and-github-tutorial/>
* https://www.atlassian.com/git/tutorials/saving-changes
