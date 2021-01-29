# Extremely short getting started with Git

- [Extremely short getting started with Git](#extremely-short-getting-started-with-git)
  - [If you already have a codebase that you need to "link" to a git repository](#if-you-already-have-a-codebase-that-you-need-to-link-to-a-git-repository)
  - [If you are creating a new repository from a remote repository.](#if-you-are-creating-a-new-repository-from-a-remote-repository)
  - [Work flow](#work-flow)
          - [Notes](#notes)


## If you already have a codebase that you need to "link" to a git repository

- Initialise 
  >`git init` 
- Confirm `user.name`, `user.email` of author for this project
  >`git config --list`  

    - Defaults are global settings
        >`git config --global --list`
- "Link" to remote repository. Default name for remote is `origin` but it can be anything. It is recommended to keep it as `origin` if you are new to `git`.
  > `git remote add origin <remote address>`
- To "sync" with remote.  
  > `git pull origin master`   

 ## If you are creating a new repository from a remote repository.

- Go to the folder where you want the working directory to be. Then run
  > `git clone <remote address>`

- By default it is on `master`. Check:
  > `git branch`

- To see remote branches:
  > `git branch -a`

- To switch, use
  > `git checkout <branchname>`


## Work flow

- To see current status of your working directory:
  > `git status`
- To commit your changes (ignore first command, if new files do not need to be added. Commit only what is necessary. Rest add to `.gitignore` file):
    > `git add <new files, if required>`
    > `git commit -am "meaningful short commit message"`
- To make changes "permanent"
    > `git push origin master`
 
 In the above cases `master` is the branch used. You may be working on a different branch.

- To see history of repository
  > `git log`



---

###### Notes

- Only basic options of important commands are discussed above. Feel free to explore, ask. I would recommend Github if you want to learn - it is not behind a VPN. It is free and on the internet. Of course **do not** use company IP code to test things there.


---------

- .gitignore
- local git repo
- git config --global --edit

converted proj folder into a git repository (local)
git init
.gitnore edit
.gitattributes
git add .gitignore
git commit -am "   "
git add *
git commit -am " "

