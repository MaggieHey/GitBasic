# Git 理解

本地文件—VScodeh—github间的传送工具

# Git 简介

> It's a version control sysytem for tracking changes in computer files.It's a distributed version control system or decentralized version control system.What that means is that many developers can work on a single peoject without having to on the same work.

它是一个版本控制系统，用于追踪电脑文件发生的改变。

它是一个分布式或分散式版本控制系统，可让不在同一网络上的开发者在同一项目上工作。

**功能包括：**

- 分布式版本控制

- 不同开发者间协同合作

- 显示何人何时做出何种改变

- 在任何时候还原文件

- 本地到远程的发布

  ![2](C:\Users\Administrator\Desktop\GitBasic\png\2.PNG)

# Git 使用简述

- 建立文件，初始化文件为仓库，运行git命令

- 使用add命令将要提交的内容放到暂存区

- 修改完毕后，将暂存区代码上传到本地仓库中

- 将本地仓库代码上传到远程仓库中，其它人可拉取信息到它们的电脑

- 多人协作时，有时会建立分支

  

# Git 常用命令

## Git 基本命令

![3](C:\Users\Administrator\Desktop\GitBasic\png\3.PNG)

## Git 命令组

准备：创建项目文件 →文件内启动Git→文件添加到VS项目→VS内添加文件→VS内进行文件编辑

```
*本地仓库+VScode*
git init //初始化该文件为仓库，可进行后续git操作
git config--global
user.name ____//输入name
git config --global user.email___//输入email
git add . //添加文件到暂存区
git status //查看暂存区内容
git commit -m '____'//将暂存区文件传到仓库
*本地仓库+远程仓库*
git remote (远程仓库链接)//连接远程仓库
git push //把本地仓库内文件传到Github
touch README.md //添加README文件
git add. //全部存到暂存区
commit add-M '____'//全部传到本地仓库
git push//本地仓库内容全部转到github


```

```
git rm --cached 文件名.属性//把文件移出暂存区
git add *.文件属性 //把该类型文件存到暂存区
```

```
touch .gitignore //不想存于仓库的文件夹
文件名.属性 //在gitignore文件中输入被移出暂存区文件名
/文件夹名 //在gitignore文件中输入被移出暂存区文件夹名
```

```
git branch ___//创建分支
git commit -m 'another change'分支上传到仓库
git checkout ____//转到分支
git .git //在分支中创建仓库
touch 文件名.属性//在分支中添加文件
git add . //将文件放到暂存区
git commit -m '____'将分支文件放到分支仓库
git checkout master //回到主支
git merge __//分支再现
```

```
git clone (项目clone链接)//把想要clone的项目放到当前文件夹
git pull //看到该项目的最新更新
```



# Github 基本建仓

- 创建新仓库

- 命名

- 简单介绍

- public和private选择

- Creek单机建仓

- readme（暂时忽略）

- 复制远程仓库Git链接

  

# Git+VScode+Github work flow

## ①四个窗口

- 文件窗口：创建本地文件

- git窗口：文件内启动git

- VS窗口：VS打开文件为项目

- Github窗口：Github建立仓库

  

## ②Git init→Git push

```
*本地仓库+VScode*
git init //初始化该文件为仓库，可进行后续git操作

git config --global user.name ____//输入name
git config --global user.email___//输入email
git add . //添加文件到暂存区
git status //查看暂存区内容
git commit -m '____'//将暂存区文件传到仓库
*本地仓库+远程仓库*
git remote (远程仓库链接)//连接远程仓库
git push //把本地仓库内文件传到Github
touch README.md //添加README文件
git add. //全部存到暂存区
commit add-M '____'//全部传到本地仓库
git push//本地仓库内容全部转到github

```

## ③Git clone + pull 

```
git clone (项目clone链接)//把想要clone的项目放到当前文件夹
git pull //看到该项目的最新更新
```

