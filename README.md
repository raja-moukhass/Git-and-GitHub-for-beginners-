<p align="center"><img width=60% src="https://github.com/raja-moukhass/Git-and-GitHub-for-beginners-/blob/master/logo/ba9a7cbd.jpeg"></p>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;

[![Build Status](https://travis-ci.org/anfederico/Clairvoyant.svg?branch=master)](https://travis-ci.org/anfederico/Clairvoyant)
![Dependencies](https://img.shields.io/badge/dependencies-up%20to%20date-brightgreen.svg)
![Dependencies](https://img.shields.io/badge/dependencies-up%20to%20date-brightgreen.svg)
[![GitHub Issues](https://img.shields.io/github/issues/anfederico/Clairvoyant.svg)](https://github.com/anfederico/Clairvoyant/issues)
![Contributions welcome](https://img.shields.io/badge/contributions-welcome-orange.svg)
[![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
# Introduction to git
### git is an Open Source Distributed Version Control System now that's a lot of words to define Git.
 - `Control System`: This basically means that Git is a content tracker. So Git can be used to store content — it is mostly used to store code due to the other features it provides
 
 - `Version Control System`: The code which is stored in Git keeps changing as more code is added. Also, many developers can add code in parallel. So Version Control System helps in handling this by maintaining a history of what changes have happened. Also, Git provides features like branches and merges, which I will be covering later.
 
 - `Distributed Version Control System`: Git has a remote repository which is stored in a server and a local repository which is stored in the computer of each developer This means that the code is not just stored in a central server, but the full copy of the code is present in all the developers’ computers. Git is a Distributed Version Control System since the code is present in every developer’s computer. I will explain the concept of remote and local repositories later in this article.
 
 - `Why a Version Control System like Git is needed`: Real life projects generally have multiple developers working in parallel. So a version control system like Git is needed to ensure there are no code conflicts between the developers.
Additionally, the requirements in such projects change often. So a version control system allows developers to revert and go back to an older version of the code.
Finally, sometimes several projects which are being run in parallel involve the same codebase. In such a case, the concept of branching in Git is very important.
# video
In this <a href="https://www.youtube.com/watch?v=uUuTYDg9XoI">video</a>  we introduce you to git and github and how it can help you collaborate on software development projects effectively.

 
 In this <a href="https://www.youtube.com/watch?v=OdbBmvfThJY">video</a> we will see :
- What is git why to use it
- Why do we need a version control system
- What is Centralised Version Control System
- What is Distributed Version Control System
- What is Trunk Based Development.

 In this first <a href="https://www.youtube.com/watch?v=BCQHnlnPusY">video</a> of Git and GitHub for Poets, we go over the concepts of commits and repositories as well as an overview of the GitHub User Interface


# get started -installing Git
- Install Git on Mac OS X
there are several ways to install on a Mac. In fact, if you've installed XCode (or it's Command Line Tools), Git may already be installed. To find out, open a terminal and enter
```
git --version
```
- install git on Linux (debian/Ubuntu)
```
sudo apt-get update
sudo apt-get install git
```
- Installing Git on CentOS
```
sudo yum -y update
sudo yum install git
```
- install git on fedora
```
sudo dnf update
sudo dnf install git
```
if you have an older version of fedora you can use the yum 
```
sudo yum update
sudo yum install git
```

- Installing Git on Windows.

For Windows, the official build is available for you to download through the Git website. Clicking <a href="https://git-scm.com/download/win">here</a> will cause the download to start automatically.

# Create your local Git repository
In your computer, create a folder for your project. Let’s call the project folder `simple-git-demo`.
Go into your project folder and add a local Git repository to the project using the following commands:

``` diff
$ mkdir raja_git
$ cd raja_git
$ git init
```
### Let’s Add some Small Code now
- Create a file called raja.txt in the project folder and add the following text into it:
``` diff
+ initial content 
```
# Staging and Committing the code

Committing is the process in which the code is added to the local repository. Before committing the code, it has to be in the staging area. The staging area is there to keep track of all the files which are to be committed.
Any file which is not added to the staging area will not be committed. This gives the developer control over which files need to be committed.
### Staging
- Use the following command for staging the file:
```
git add raja.txt
```
In case you want to add multiple files you can use:
``` diff
+ git add file1 file2 file3
```

If you want to add all the files inside your project folder to the staging area, use the following command:

```diff
$ git add .
- or
$ git add *
- or
$ git add -A
- or 
$ git add -all
```
### commiting
“Initial Commit” is the commit message here. Enter a relevant commit message to indicate what code changes were done in that particular commit.
```
git commit -m "Initial commit"
```
### status 

Use `git status` to find out information regarding what files are modified and what files are there in the staging area — it shows other information as well, which we can ignore for now.

- Use the following command to see the status:
```
git status
```
The status shows that demo.txt is modified and is not yet in the staging area.

Now let us add demo.txt to the staging area and commit it using the following commands:

```
$ git add demo.txt 
$ git commit -m "demo.txt file is modified"
```

### Log
use `git log`  to print out all the commits which have been done up until now.
the command used for this is .

```
git log
```
The log shows the author of each commit, the date of the commit, and the commit message.

# branches

### what is a branch 













