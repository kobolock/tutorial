# Tutorial


First steps with Atom editor
============================

Create a repo on Github and find it on Atom
-------------------------------------------
  * Create a account Github
  * Create a new repo (alias project, for example "tutorial")
  * Copy URL project
  * From Atom, CTRL+SHIFT+p for open option research command
  * Enter "Github:clone", select this one
  * Paste the URL project, and store into the directory. By default, on windows `C:\Users\[user_name]\Github`
  * Project appears in a new window  

Authorize for Atom
------------------
  * Go to `github.atom.io\login` to generate an authentication token
  * Copy the token Github
  * From Atom, in Github window, paste the token to login

How push a new file or modified file
------------------------------------
  * From the README.md file, add new comments
  * Save file with CTRL+S
  * File appears in the Git window, in the "Unstaged Changes"
  * Add info commit. For example, "Add new comments in README.md"
  * Click on "Commit to master"

Note : If Git is not already installed on your machine, a error message appears.
Please, install Git before commit and, open terminal to enter `git config --global user.email "user.email"` and `git config --global user.name "user.name"`

Supplemental infos
------------------
[How to connect Github with Atom] (https://youtu.be/6HsZMl-qV5k)


Adding an existing project to GitHub
====================================

  * Create a new repo from Github
  * Open Github
  * Change directory  
    `$ cd /F/workspace/git_repo/test_repo/`
  * Initialize the local directory  
    `$ git init  
    Initialized empty Git repository in F:/workspace/git_repo/test_repo/.git/`
  * Add files in the new local directory  
    `$ git add .`
  * Commit the files  
    `$ git commit -m "initial commit"  
    [master (root-commit) a0cceb9] initial commit  
    1 file changed, 1 insertion(+)  
    create mode 100644 test.txt`
  * Copy the remote repository URL,  add the URL for the remote repository where your local repository will be pushed.  
  `$ git remote add origin https://github.com/kobolock/testrepo.git`  
  * Initialize the local directory   
  `$ git remote -v  
  origin  https://github.com/kobolock/testrepo.git (fetch)  
  origin  https://github.com/kobolock/testrepo.git (push)`  
* Push the changes in your local repository to GitHub.
  `$ git push origin master  
  Enumerating objects: 3, done.  
  Counting objects: 100% (3/3), done.  
  Writing objects: 100% (3/3), 217 bytes | 217.00 KiB/s, done.  
  Total 3 (delta 0), reused 0 (delta 0)  
  To https://github.com/kobolock/testrepo.git  
  * [new branch]      master -> master`  
