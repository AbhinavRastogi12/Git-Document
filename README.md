# Git-Document

<pre>
<strong>What is git?</strong>

It is a distributed version control system, which track files.

<strong>why we use git?</strong>

Easily recover files,

who introduce an issue and when,

Roll back to previously working state.

<strong>History</strong>

-> Local vcs 

pros-> can track files and rollback

cons-> if you lost your harddisk everything is lost

-> Centralized vcs

pros-> you can track files

cons-> if server damage you can't rollback

-> Distributed vcs 

pros-> secure backup


<strong>Three Stage Architecture</strong>

-> working directory

-> staging area

-> git directory(repository)


<strong>Basic Commands</strong>

-> git config --global user.name "username"                                    //to configure username

-> git config --global user.email "useremail"                                  //to configure useremail

-> git status                                                                  //to check status of directory

-> git init                                                                    //to intialise git
 
-> git add --a                                                                 //to store all files in staging area 

-> git add filename.extention                                                  //to add single file

-> git add .                                                                   //to add all files

-> git commit -m "Initial commit"                                              //to commit changes

-> git log                                                                     //to check all commits

-> git log -p                                                                  //to check all commits along with all removes

-> git log --stat                                                              //to check short summary about all commits

-> git clone                                                                   //to create clone of git repository

-> git diff                                                                    //to compare working directory with staging area

-> git diff --staged                                                           //to compare last commit with staging area

-> git commit -a -m "Direct commit"                                            //to skip staging area(note:- this command commit's only tracked files, untracked files cannot be commited through this command)

-> git clone url.git foldername                                                //to clone git repository into folder(note:- when you mention foldername after url.git, the repository will clone into that folder) 

-> git log --pretty=short                                                      //to check the author of directory

-> git log --pretty=full                                                       //to check the author and commiter of directory(note:- author is one who create first file, and commiter is who change or add new the files)

-> git restore --staged filename.extention                                     //to unstage file

-> git checkout -f                                                             //to rollback whole directory into last commit

-> git checkout -- filename.extention                                          //to rollback into last commit

-> git remote -v                                                               //to check form where to pull or push 

-> git remote add origin https://github.com/username/repositoryname.git        //to create remote origin

-> git push -u origin master(branch name)                                      //to push directory to repository


<strong>Git Ignore(.gitignore)</strong>

Git ignore(.gitignore) is use to ignore the files, when you put files in ".gitignore" folder, you won't be able to track those files.


Linux Commands

-> pwd                                           //to check present working directory

-> ls                                            //to list content

-> dir                                           //to check the number of directories in folder

-> mkdir file.extention                          //to create new directory                          

-> cd                                            //to change directory 

-> git rm -rf .git                               //to remove entire repository(execute at your own risk)

-> git rm filename.extention                     //to remove file

-> git mv oldname newname                        //to rename the folder

-> touch filename.extention                      //to create file


<strong>SSH key</strong>

-> ssh-keygen -t rsa -b 4096 -C "your_email@example.com"       //to generate ssh key

-> eval `ssh-agent -s`                                         //to generate agent pid

For more info about ssh key visit "https://docs.github.com/en/github/authenticating-to-github/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent"      

<strong>Alias in git</strong>

Alias in git is use to give alias name, with the help of alias you can create shortcut for commands

Example:-

-> git config --global alias.st status     //new command to check git status is "git st"

For more info you can visit "https://git-scm.com/book/en/v2/Git-Basics-Git-Aliases"

<strong>Branches/Merging in git</strong>

-> git branch                       //to check branches
-> git checkout -b newbranchname    //to create new branch 
-> git merge newbranchname          //to give merge request
-> git branch -d branc              //to delete branch

In Git, branches are a part of your everyday development process, when you create your own branch you can do work without effecting existing master/main branch.
</pre>
