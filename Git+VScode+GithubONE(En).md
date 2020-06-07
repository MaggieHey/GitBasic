# 1.1 Git understanding



A Transfer tool during 

**local files-VScode-github** 

# 1.2 Git introduction

> It's a version control sysytem for tracking changes in computer files.It's a distributed version control system or decentralized version control system.What that means is that many developers can work on a single peoject without having to on the same work.

**Features include:**

- Distributed version control
- Coordinates work between multiple 
- developers 
- Who made what changes and when
- Revert back at any time
- Local&remote repos     





# 1.3 Git simple use summary


- Create a folder and initialize the folder as a repository
- Use the add command to put the content to be submitted to the the temporary storage area 
- After the modification, upload the code in the temporary storage area to the local repository
- Upload the local repository code to the remote repository, others can pull the information to their computers
- When multiple people collaborate, sometimes branches are created



# 1.4 Git common commands

## Git 基本命令

![](https://ftp.bmp.ovh/imgs/2020/06/2911d3f20f9e5638.png)

## Git 命令组

Preparation: Create a project folder → Start Git in the folder → Add files to the VS project → Add folders in VS → Edit files in VS

```
*Local repository+VScode*
git init //Initialize the folder as a repository, you can perform subsequent git operations
git config--global
user.name ____//input name
git config --global user.email___//input email
git add . //Add file to staging area
git status //View staging area files
git commit -m '____'//Transfer files from the staging area to the repository
*local repository+remote repository*
git remote (remote repository URL)//link remote repository
git push //Transfer files from local repository to Github
touch README.md //add README file
git add. //Save all to the staging area
commit add-M '____'//All to local repository
git push//The contents of the local repository are all transferred to github


```

```
git rm --cached 
file name.Attributes//move the file out of the staging area
git add *. attributes//Save this type of file to the staging area
```

```
touch .gitignore //Files that do not want to be stored in the repository
file name.attributes // input the file name to be moved out of the staging area in gitignore file
/folder name //input the folder name to be moved out of the staging area in gitignore file
```

```
git branch ___//create branch
git commit -m 'another change'Upload the branch to the repository
git checkout ____//go to branch
git .git //Initialize the repository in the branch
touch file name.attributes//add file in the branch 
git add . //put the file in the staging area
git commit -m '____'put the files of branch to the repository of branch
git checkout master //go back to master
git merge __//merge branch
```

```
git clone (project clone link)//Put the item you want to clone into the current folder
git pull //see the latest update of the project
```



# 1.5 Git repository establishment


- Create a new repository

- name

- basic introduction

- public and private options

- Creek ！

- readme (ignore for now)

- Copy Git link to remote repository

# 1.6 Git+VScode+Github work flow

## ①Four windows

- folder window：create local files

- git window：four windows

- VS window：VS opens the folder as a project

- Github window：Github create repository

  

## ②Git init→Git push

```
*local repository+VScode*
git init //Initialize the folder as a repository, you can perform subsequent git operations

git config --global user.name ____//input name
git config --global user.email___//input email
git add . //Add file to staging area
git status //View staging area files
git commit -m '____'//Transfer files from the staging area to the repository
*local repository+remote repository*
git remote (remote repository link)//link remote repository
git push //Transfer files from local repository to Github
touch README.md //add README file
git add. //Save all to the staging area
commit add-M '____'//All to the local repository
git push//The contents of the local repository are all transferred to github

```

## ③Git clone + pull 

```
git clone (project clone link )//put the item you want to clone into the current folder
git pull //see the latest update of the project
```

