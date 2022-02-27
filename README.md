[![Git](https://i.imgur.com/9cCzCdY.png "Git")](https://git-scm.com/ "Git")
### Table of Contents

[TOCM]


Git
===
Git is the most commonly used version control system. Git tracks the changes you make to files, so you have a record of what has been done, and you can revert to specific versions should you ever need to. Git also makes collaboration easier, allowing changes by multiple people to all be merged into one source. 

So regardless of whether you write code that only you will see, or work as part of a team, Git will be useful for you.

![](https://i.imgur.com/UmkYZFK.png)

Git is software that runs locally. Your files and their history are stored on your computer. You can also use online hosts (such as [GitHub](https://github.com/ "GitHub") or [Bitbucket](https://bitbucket.org/ "Bitbucket")) to store a copy of the files and their revision history. Having a centrally located place where you can upload your changes and download changes from others, enable you to collaborate more easily with other developers. Git can automatically merge the changes, so two people can even work on different parts of the same file and later merge those changes without losing each others work!


Version Control System
=============
You can think of a version control system (short: “VCS”) as a kind of“database”. It lets you save a snapshot of your complete project at any time you want. When you later take a look at an older snapshot (let's start calling it“version”), your VCS shows you exactly how it differed from the previous one.

![](https://i.imgur.com/u9lC5qq.jpg)

Version control is independent of the kind of project / technology / framework you are working with:
- It works just as well for an HTML website as it does for a design project or
an iPhone app
- It lets you work with any tool you like; it doesn‘t care what kind of text
editor, graphics program, file manager or other tool you use
Also, don‘t confuse a VCS with a backup or a deployment system. You don‘t have to change or replace any other part of your tool chain when you start using version control.<br>
A version control system records the changes you make to your project‘s files. This is what version control is about. It‘s really as simple as it sounds.

## Version Control Benefits 
There are many benefits to version control. The biggest benefits of the right VCS include:

- A single source of truth across teams, code, and assets.
- Traceability for every change ever made.
- Speed for development teams who don't want to waste time looking for a file.

Getting Started
==========
# Installing Git
## Windows
####  Download Git for Windows
1. Browse to the official Git website: https://git-scm.com/downloads
2. Click the download link for Windows and allow the download to complete.

![](https://i.imgur.com/mMKbDNu.png)

#### Extract and Launch Git Installer
3 . Browse to the download location (or use the download shortcut in your browser). Double-click the file to extract and launch the installer.

![](https://i.imgur.com/OcsTh69.png)

 4 . Allow the app to make changes to your device by clicking **Yes** on the User Account Control dialog that opens.

![](https://i.imgur.com/uTpIa1L.png)

 5 . Review the GNU General Public License, and when you’re ready to install, click **Next**.

![](https://i.imgur.com/Wd1Vcxs.png)

 6 . The installer will ask you for an installation location. Leave the default, unless you have reason to change it, and click **Next**.

![](https://i.imgur.com/1u7t3W3.png)

 7 . A component selection screen will appear. Leave the defaults unless you have a specific need to change them and click **Next**.

![](https://i.imgur.com/XI0JIy2.png)

 8 . The installer will offer to create a start menu folder. Simply click **Next**.

![](https://i.imgur.com/o8mN6Rp.png)

 9 . Select a text editor you’d like to use with Git. Use the drop-down menu to select Notepad++ (or whichever text editor you prefer) and click **Next**.

![](https://i.imgur.com/sIRCDTz.png)

 10 . The next step allows you to choose a different name for your initial branch. The default is 'master.' Unless you're working in a team that requires a different name, leave the default option and click **Next**.

![](https://i.imgur.com/8pB5NoV.png)

 11 . This installation step allows you to change the **PATH environment**. The **PATH** is the default set of directories included when you run a command from the command line. Leave this on the middle (recommended) selection and click **Next**.

![](https://i.imgur.com/TgMjc46.png)

#### Server Certificates, Line Endings and Terminal Emulators
 12 . The installer now asks which SSH client you want Git to use. Git already comes with its own SSH client, so if you don't need a specific one, leave the default option and click **Next**.

![](https://i.imgur.com/8V73PCP.png)

 13 . The next option relates to server certificates. Most users should use the default. If you’re working in an Active Directory environment, you may need to switch to Windows Store certificates. Click **Next**.

![](https://i.imgur.com/jLu0LTz.png)

 14 . The next selection converts line endings. It is recommended that you leave the default selection. This relates to the way data is formatted and changing this option may cause problems. Click **Next**.

![](https://i.imgur.com/3ZNpoHV.png)

 15 . Choose the terminal emulator you want to use. The default MinTTY is recommended, for its features. Click **Next**.

![](https://i.imgur.com/Godf6n1.png)

 16 . The installer now asks what the `git pull` command should do. The default option is recommended unless you specifically need to change its behavior. Click **Next** to continue with the installation.

![](https://i.imgur.com/EJdVW0E.png)

 17 . Next you should choose which credential helper to use. Git uses credential helpers to fetch or save credentials. Leave the default option as it is the most stable one, and click **Next**.

![](https://i.imgur.com/1U8FwAw.png)

#### Additional Customization Options
 18 . The default options are recommended, however this step allows you to decide which extra option you would like to enable. If you use symbolic links, which are like shortcuts for the command line, tick the box. Click **Next**.

![](https://i.imgur.com/uClHvXi.png)

 19 . Depending on the version of Git you’re installing, it may offer to install experimental features. At the time this article was written, the options to include support for pseudo controls and a built-in file system monitor were offered. Unless you are feeling adventurous, leave them unchecked and click **Install**.

![](https://i.imgur.com/gGACFNn.png)

#### Complete Git Installation Process
 20 . Once the installation is complete, tick the boxes to view the Release Notes or Launch Git Bash, then click **Finish**.

![](https://i.imgur.com/fDfUnVX.png)

Configuring Git
==========
### Launch Git Bash Shell
To launch Git Bash open the Windows Start menu, type git bash and press Enter (or click the application icon).

![](https://i.imgur.com/CBfBuxU.png)

Now that you have git installed, it is a good idea to set up your personal information that will be used when you commit your code.

The following commands will set your git commit **username** and **email address**:
```shell
git config --global user.name "Your Name"
git config --global user.email "youremail@yourdomain.com"
```
To verify the configuration changes, type:
```shell
git config --list
```
The output should look something like this:

![](https://i.imgur.com/cJXMjOO.png)

Git- Three Stage Architecture
==================
First of all, let us have a look at a two stage architecture Version Control System.

![](https://i.imgur.com/y42N1uA.png)

In a two stage Version Control System, we work on our working directory, commit some changes and then push to the repository. Then again, we can pull the changes from the repository (changes which might have done by our colleagues), commit some changes, and again push back the files to the repository.

Till now, it seems very good, but now imagine a situation, when you are working on a project consisting of say 4 files. Now, you have finished working on 2 files, but in other 2 files, you have encountered some bug. In such situation, if you commit changes to the repository, then the other two files containing bug will also be committed to the repository. This is a serious problem!

But git solves this problem by introducing a middle stage called “staging area” in this architecture. Let us have a look at three stage architecture now.

![](https://i.imgur.com/FPPyXif.png)

Thus, git allows us to first push our files to staging area, and then we can commit those staged files. Continuing our above example, we can only push those two bug-free complete files to staging area and then further commit our changes. The other two files in progress can remain in our working directory. They can be modified later and committed when you need to. Another important advantage of staging area is that files from staging area can again be pulled to our working directory, if we feel they need some more changes before committing them.

**It is to be noted that it is not compulsory in git to first push the files to staging area. The changes can even be directly committed, but it is always a good practice to first stage our files.**

Tracking Our first Git Project
==================
Let’s say we have 2 files in a folder for which we want to create a git repository. So follow these steps to track these files using git.

- Open the folder, Right-Click anywhere while shifting and choose **Git Bash Here**.

![](https://i.imgur.com/v38uQQE.png)

- After Git bash is opened type “**git status**”.

```shell
git status
```
![](https://i.imgur.com/nenKgrK.png)

- It will give you a message that “fatal: not a git repository (or any of the parent directories): .git”.

- It is a message that says these files are not considered as a git repository.

- Now we will type “**git init**” to initialize this folder as a repository.

```shell
git init
```

![](https://i.imgur.com/91AvPqR.png)

- Now if we type “**git status**” then we will get the files which are present in the folder. Also, it says there that the files are not tracked.

```shell
git status
```
![](https://i.imgur.com/MLoVx5X.png)

- Now to track all the files inside this got repository we will type  **git add - -a** , which will add all these files to the staging area.

```shell
git add - -a
```
![](https://i.imgur.com/WcAI0ln.png)

- Now if we type **git status** then says there that all the files tracked but not commit yet.

```shell
git status
```
![](https://i.imgur.com/wsoMWdO.png)

- Now we have to commit using this command **git commit -m “Initial Commit”**.

```shell
git  commit -m "Initial Commit"
```
![](https://i.imgur.com/apZHb7i.png)

- Now if we do **git status** again it will say There’s nothing to commit, working tree clean. Which means we have successfully tracked our files.

```shell
git status
```
![](https://i.imgur.com/hSjoNOO.png)

- Now to see the commits we have made, we will use **git log** command.

```shell
git log
```

![](https://i.imgur.com/q8O1Bve.png)

- Now if we modify a single file and want to stage that only file we will use **git add file.ext** (Where file.ext is the filename and extension).

![](https://i.imgur.com/frVAQCN.png)

```shell
git add File1.txt
```
![](https://i.imgur.com/PxgB58d.png)

- Now we will commit with a message by typing **git commit -m “Your commit message”**

```shell
git  commit -m "Second Commit"
```
![](https://i.imgur.com/0TDcY19.png)

- Done Now You have successfully tracked your files.

Cloning a Remote Git Repository from GitHub
=============================
- Open Browser and go to the GitHub page of that git repository.

![](https://i.imgur.com/n9AhhYe.png)

- Now click on code or download and copy the URL.

![](https://i.imgur.com/o3zgTMx.png)

- Open git bash and type `git clone (copied URL)`

```shell
git clone https://github.com/basitaminbhatti/Udacity-AI-Programming-with-Python.git
```
- Wait for the git clone to complete, this will only take a little bit of time for the first time.

![](https://i.imgur.com/TIsAQLi.png)

- Now you can change the files locally, track them also commit them locally.

File Status Lifecycle
============
When you start to track files on an empty repository every file stays in the untracked stage. Which means we have not staged these files. So after adding the files by typing `git add --a`, every file moves into the unmodified section. Now if we change a few files they will be moved to modified and staged. Now what happened here is, we have added every file to the tracker and now as we modify files will be moved to the modified phase. Now if we run the add command then the files which were in the modified stage will be staged.

- Let’s open a new folder and initialize as a git repo by opening Git bash and typing `git init`
- Now lets add the files by using `git add --a`
- Now every file has been staged.
- Now if we change 1 file and do `git status` then you will see that the file we changed is present both on staging area and untracked area. Because you have staged the file and those are meant to go to the commit until the user stages other changes. So only those will go to the next commit which are staged. The untracked files will be ignored unless the user adds them to stage.

![](https://i.imgur.com/pAm1dh1.png)


Gitignore
=================
### Introduction
When you make commits in a git repository, you choose which files to stage and commit by using `git add FILENAME` and then `git commit`. But what if there are some files that you never want to commit? It's too easy to accidentally commit them (especially if you use `git add .` to stage all files in the current directory). That's where a `.gitignore` file comes in handy. It lets Git know that it should ignore certain files and not track them.

### .gitignore File
The `.gitignore file` is a text file that tells Git which files or folders to ignore in a project.

A local .gitignore file is usually placed in the root directory of a project. You can also create a global `.gitignore` file and any entries in that file will be ignored in all of your Git repositories.

To create a local `.gitignore` file, create a text file and name it `.gitignore` (remember to include the `.` at the beginning). Then edit this file as needed. Each new line should list an additional file or folder that you want Git to ignore.

The entries in this file can also follow a matching pattern.

- `*` is used as a wildcard match
- `/` is used to ignore pathnames relative to the .gitignore file
- `#` is used to add comments to a .gitignore file

This is an example of what the `.gitignore` file could look like:
    # Ignore Mac system files
    .DS_store
    
    # Ignore node_modules folder
    node_modules
    
    # Ignore all text files
    *.txt
    
    # Ignore files related to API keys
    .env
    
    # Ignore SASS config files
    .sass-cache
### Adding .gitignore to your repo and ignore files:
- Let’s start by creating an unnecessary file. 
- Open git bash on that folder and type `touch file.log`

```shell
touch file.log
```
![](https://i.imgur.com/6ekDkLc.png)

- Now you will see file.log will be created.

![](https://i.imgur.com/WhfUn2m.png)

- Now we will gitignore this file.
- Again open git bash and type `touch .gitignore`

```shell
touch .gitignore
```

![](https://i.imgur.com/1UBetTs.png)

- Now if you do `git status` it will return you 2 untracked files, .gitignore and file.log.

```shell
git status
```

![](https://i.imgur.com/4BvUZWW.png)

- Now let’s open `.gitignore` file using notepad, type there file.log and save and close it.

![](https://i.imgur.com/jg54IDE.png)

- Now if we do `git status` it will return only 1 file, which is .gitignore. Because the other one will be ignored.

```shell
git status
```
![](https://i.imgur.com/bisrv9F.png)

- Now type `git add --a` to add gitignore to the staging area.

```shell
git add - -a
```

![](https://i.imgur.com/WcAI0ln.png)

- Now let’s commit by typing `git commit -m “added .gitignore”`

```shell
git  commit -m "added .gitignore"
```

![](https://i.imgur.com/5HINTR7.png)

- Done! We have successfully created .gitignore for our repo. 

### Ignoring Specific Extension files:
- Create .gitignore the same as the last one.
- Now open it using notepad and type there `*.extension` to ignore. **(example for ignoring .log files : “*.log”)**

![](https://i.imgur.com/LYBpA9C.png)

- Now save and exit the notepad and commit the gitignore to your repo.

### Ignoring Folders:
- Now we will ignore a whole directory.
- Create and open .gitignore and type there the directory name followed by `\` **(example: dir/ )**

![](https://i.imgur.com/uh4LoRf.png)
- If you create a blank folder, git will automatically ignore it.

Git Diff
=====
Showing Changes Between Commits/Staging Area & Working Directory
 <hr>
### What is Git Diff?
 
Diff command is used in git to track the difference between the changes made on a file. Since Git is a version control system, tracking changes is a very vital part to it. Diff command takes two inputs and shows the differences between them. These inputs can be branches, working trees, commits and more. Now Let’s learn about Git Diff in these simple steps.
-  Let’s start by staging one file. 
- Open git bash on that folder and add that file into the staging area by typing `git add --a`

```shell
git add - -a
```

![](https://i.imgur.com/3T7l383.png)

- Now if you do `git status` it will show that the file has been staged.

```shell
git status
```

![](https://i.imgur.com/9UylG4Z.png)

- Now if you modify the file and do `git status` , it will show that the file has been modified and not staged for commit and also it will show that the file is ready to be committed.

```shell
git status
```

![](https://i.imgur.com/2SCqGcE.png)

Why does it happen? It happens only because we have staged the file earlier so it has moved to the staging area and is ready to be committed, and when we have modified it, it also shows up on the modified area. We have seen this happen earlier too. 

- Now let’s compare the working directory with the staging area so we can see those changes.
- Type `git diff` and see the output.

```shell
git diff
```

- The output should look like this.

![](https://i.imgur.com/WBG80DC.png)

- Now if we do `git add --a` and do `git diff` it will show nothing because we have staged every change.



### Examine Git Diff Output
 Let us now examine a more detailed breakdown of the diff output.
####  1. Comparison input

![](https://i.imgur.com/iZBvqiX.png)

This line displays the input sources of the diff. We can see that `a/File1.txt` and `b/File1.txt` have been passed to the diff.

####  2. Meta data

![](https://i.imgur.com/7rzN5UB.png)

This line displays some internal Git metadata. You will most likely not need this information. The numbers in this output correspond to Git object version hash identifiers.

####  3. Markers for changes
![](https://i.imgur.com/dYfrTR4.png)

These lines are a legend that assigns symbols to each diff input source. In this case, changes from `a/File1.txt` are marked with a - - - and the changes from `b/File1.txt` are marked with the +++ symbol.

####  4. Diff chunks
The remaining diff output is a list of diff 'chunks'. A diff only displays the sections of the file that have changes. In our current example, we have chunks as we are working with a simple scenario. Chunks have their own granular output semantics.

  ![](https://i.imgur.com/RfvaLYw.png)

The first line is the chunk header. Each chunk is prepended by a header inclosed within **@@ symbols.** The content of the header is a summary of changes made to the file.
  ![](https://i.imgur.com/qGCjbDs.png)

In this header example, **7** lines have been extracted starting from line number **3**. Additionally, **7** lines have been added starting at line number **3**.

The remaining content of the diff chunk displays the recent changes. Each changed line is prepended with a `+` or `-` symbol indicating which version of the diff input the changes come from. As we previously discussed, `-` indicates changes from the `a/File1.txt` and `+` indicates changes from `b/File1.txt`

### Git Diff in previous commits:
- If we use `git diff --staged` it will compare every commit with your working directory.

```shell
git diff --staged
``` 

![](https://i.imgur.com/naFBTke.png)

Skipping The Staging Area
================
- Let’s modify a file in our directory.
- Now open git bash in that directory. 
- If we do `git status` it will show us that the file has been modified but not has been staged.

```shell
git status
```

![](https://i.imgur.com/Oe0aDae.png)

- Let’s create a new file on that directory and do `git status`

```shell
git touch file3.txt

```
![](https://i.imgur.com/OQyZDqB.png)

```shell
 git status
```
![](https://i.imgur.com/a9cdZ8Z.png)

- It will show us that the tracked file (the file we modified earlier) has been modified but not added to the staging area and the new file is untracked.

- Now let’s skip the staging and directly commit.

- **NOTE:** Only tracked files can skip the staging area, to add your file to tracker type `git add --a` **or** `git add filename.extension`

- Now let's skip the staging by typing `git commit -a -m “Direct commit”`

```shell
git commit -a -m “Direct commit”
```
![](https://i.imgur.com/IxFtkz5.png)

- Now if we do `git status` it will show that the working directory is clean. Which means we have successfully skipped the staging area and committed the changes.

```shell
git status
```

![](https://i.imgur.com/vNANPw3.png)

Moving and Renaming Files
=================
We can also do it manually but then, we need to stage those changes using git bash. That is why we are going to do it inside git. Git will automatically stage it after **moving/deleting/renaming** that file. So let’s get started.
### Deleting Files:
To delete files using git we need use this command: `git rm filename.extension` It will delete the file and if you do `git status` now it will say that the file has been deleted and staged. Now we can commit it by using the “git commit -m “commit message”” command.

```shell
git rm file3.txt  # where file name is file3.txt
```
![](https://i.imgur.com/5aIyf6d.png)

```shell
git status
```
![](https://i.imgur.com/oaL85wL.png)

### Renaming Files:
To rename file we need to use this command : `git mv filename.extension renamefile.extension` It will rename the file from **filename.extension** to **renamefile.extension**. And it will also get automatically staged by git. All we need to do is commit.

```shell
 git mv File1.txt NewFileName.txt
```

![](https://i.imgur.com/HWCirdG.png)

### Untracking Tracked Files:
The Git rm –cached flag removes a file from the staging area. The files from the working directory will remain intact. This means that you’ll still have a copy of the file locally. The file will be removed from the index tracking your Git project.

To untrack a specific file we need to use `git rm --cached file.extension` command. It will remove that file from the tracker and it will become an untracked file.

```shell
git rm --cached IGo.txt
```

![](https://i.imgur.com/GjU77lF.png)

Git Log
=====
### Commits History:
To see the commits made on the git repo, we need to type `git log` After typing this you can see the commits that have been made on the repo.

```shell
 git log
```
![](https://i.imgur.com/Otoz7Ww.png)

**Output:**
![](https://i.imgur.com/brU3fWS.png)

To exit we need to type “**q**” on our keyboard and press enter.

### Diff in Commits:
To see the Diff in a commit we need to use `git log -p` It will show what has been changed on a commit.

```shell
git log -p
```
![](https://i.imgur.com/ywPO9KN.png)

**Output:**
![](https://i.imgur.com/Cqc9Btq.png)

###  Specific No Commits with Changes:
To see specific no commits with changes we need to use `git log -p -2` (for seeing the last 2 changes).
```shell
git log -p -2
```
![](https://i.imgur.com/SbUe1TZ.png)
### Brief Summary:
We can get a brief summary of commits by typing `git log --stat`
```shell
git log --stat
```
![](https://i.imgur.com/R6qsUT1.png)

**Output:**
![](https://i.imgur.com/7G7LHte.png)

### Customized Commit Output:
#### Pretty
- ##### One Line
If you want to see the commits on one line then type `git log --pretty=oneline`

```shell
git log --pretty=oneline
```
![](https://i.imgur.com/RSK7drw.png)

**Output:**

![](https://i.imgur.com/6BXhMW4.png)

- ##### Short
If you just want to see the commits and The author then use `git log --pretty=short`

```shell
git log --pretty=short
```
![](https://i.imgur.com/NhD5PNI.png)

**Output:**

![](https://i.imgur.com/YpiJfYN.png)

- ##### Full
If you want a little bit more info like who is the committer, commit message, then use `git log --pretty=full`

```shell
git log --pretty=full
```
![](https://i.imgur.com/SXZzoXQ.png)

**Output:**

![](https://i.imgur.com/JUMEayD.png)

- ##### Format
We can format the output by using the formatting  codes provided in [Gits](https://git-scm.com/docs/git-log#:~:text=Placeholders%20that%20expand%20to%20information%20extracted%20from%20the%20commit%3A "Gits") website.
**Example:**
we can use this format to print just the author name and the hash : `git log --pretty=format:“%h --%ae”`

```shell
git log --pretty=format:“%h --%ae”
```
![](https://i.imgur.com/r6w98cG.png)

#### Since
- ##### Weeks
If you want to filter commits by time, then use this command, `git log --since=2.weeks` to see the last 2 weeks of data.

```shell
git log --since=2.weeks
```
![](https://i.imgur.com/3OnKT0v.png)

**Output:**
![](https://i.imgur.com/sccusUV.png)

- ##### Months
To see the last 2 months of data type `git log --since=2.months`

```shell
git log --since=2.months
```
![](https://i.imgur.com/rxnOZ8G.png)

**Output:**
![](https://i.imgur.com/sccusUV.png)

### Changing A Commit Message:
Now to change a commit. So, to change the most recent commit we need to type `git commit --amend` and press enter.

```shell
git commit --amend
```

![](https://i.imgur.com/ZaMxbjN.png)

Then an editor will open where you can change the commit message. All you need to do is change the message and then you need to close it

![](https://i.imgur.com/PxQk9Kg.png)

 All you need to do is change the message and then you need to close it
 
![](https://i.imgur.com/lpOtID4.png)

by pressing i then esc key then type **“:wq” **to exit the editor. Now you have successfully edited the commit.

![](https://i.imgur.com/ayiBE9W.png)

Unstaging
======
Let’s say we have few files in our git repository and we have staged them. 

![](https://i.imgur.com/nHLl0QN.png)

Now for some reason we want to unstage a file.  Let’s see.
- To unstage a file use `git restore --staged file.ext` It will unstage the file.

```shell
git restore --staged file.log
```
![](https://i.imgur.com/1XoitN7.png)

- Now you can verify it by using `git status`

```shell
git status
```

![](https://i.imgur.com/hAVOo5d.png)

Unmodifying
========

- Now let’s say we have modified the unstaged file and made some changes which were not necessary.

![](https://i.imgur.com/TVQznzg.png)

- Now the program is not working. So we have to restore that file to its previous state where it was working. To do it use `git checkout -- file.ext`

```shell
git checkout -- file.log
```
![](https://i.imgur.com/DzGsOAd.png)

- Now git will restore that file to its last commit state.

```shell
git status
```

![](https://i.imgur.com/XhN1IfC.png)

------------
- To restore your entire working directory to the previous commit use `git checkout -f` It will restore your entire directory to the last commit.

![](https://i.imgur.com/zzW0HIn.png)

```shell
git checkout -f
```
![](https://i.imgur.com/2mhyszJ.png)

- Now If we check the status entire working directory restore to the previous commit.

```shell
git status
```
![](https://i.imgur.com/WlromYl.png)

[![GitHub](https://i.imgur.com/w47k9l7.png "GitHub")](https://github.com/ "GitHub")


GitHub
====
GitHub is a website and cloud-based service that helps developers store and manage their code, as well as track and control changes to their code. To understand exactly what GitHub is, you need to know two connected principles:

- Version control
- Git


Create A Github Account
===============
- **Step # 1:** Goto **[GitHub](https://github.com/ "GitHub") ** Website.

[![GitHub](https://i.imgur.com/G0Tj1o7.png "GitHub")](https://github.com/ "GitHub")

- **Step # 2:**  Click on "**Sign up for Github**" button.

![](https://i.imgur.com/uUjACdd.png)

- **Step # 3:** 
	 - Enter your valid email address and password which you want to give.
	 - Enter username of your choice (you can change your username later)(choosing a name which is easily remembered, short and professional looking is useful) (in the end it's your choice to pickup your username)
	 - Enter y or n in next field according to your choice if you want to receive promotional emails from GitHub (I prefer to choose n)
	 - Resolve a captcha and click on create account

![](https://i.imgur.com/lV2jHt1.png)

- **Step # 4:**  Next you will need to add the code received on your entered email address.

![](https://i.imgur.com/IT59Yo2.png)

- **Step # 5:**  After that you will be prompted to answer some question.
- **Step # 6:**  Choose just me or 2-5 option & Student (as we are student right now, you can choose developer if you are not student)

![](https://i.imgur.com/U2ROc6b.png)

- **Step # 7:**  Choose some features which you are interested in using? or looks interesting to you.

![](https://i.imgur.com/UuhXvDE.png)

- **Step # 8:**  After that choose the free option

![](https://i.imgur.com/ftXtgog.png)

- **Step # 9:**  Once you see the similar screen as below then it means you have created your GitHub account successfully.

![](https://i.imgur.com/hbmspgM.png)


Set up SSH authentication with GitHub
=======================
Adding an SSH key to GitHub allows you to pull and push data without typing in your password all the time. First we'll copy the key we generated in the Create an SSH Key step and add it to your GitHub account.

- **Step # 1:**  Go to your account settings on github.

[![GitHub Profile Setting](https://i.imgur.com/YjF9s6y.png "GitHub Profile Setting")](https://github.com/settings/profile "GitHub Profile Setting")

- **Step # 2:**  Then SSH and GPG keys.

[![SSH Keys](https://i.imgur.com/h8xL53H.png "SSH Keys")](https://github.com/settings/keys "SSH Keys")

- **Step # 3:**  Then click on the new SSH key.

[![SSH Keys](https://i.imgur.com/uD4PZlw.png "SSH Keys")](https://github.com/settings/keys "SSH Keys")

- **Step # 4:**  Add a title. Now for the key.

![](https://i.imgur.com/OZEEQDl.png)

- **Step # 5:**  Open git bash and follow the simple steps.

- **Step # 6:**  On git bash type the following edit your email and press enter: `ssh-keygen -t rsa -b 4096 -C "your_email@example.com" `

```shell
ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
```
![](https://i.imgur.com/IXOUJr4.png)

- **Step # 7:**  Now just simply press enter 3 times.

**Output:**
![](https://i.imgur.com/NQ3ncmL.png)

- **Step # 8:**  Now run this command `eval $(ssh-agent -s)`

```shell
eval $(ssh-agent -s)
```
![](https://i.imgur.com/7nyG5VM.png)

- **Step # 9:**  Now run this `ssh-add ~/.ssh/id_rsa`

```shell
ssh-add ~/.ssh/id_rsa
```
![](https://i.imgur.com/GKiO0lU.png)

- **Step # 10:**  Now on git bash type this to reveal your key `tail ~/.ssh/id_rsa.pub`

```shell
tail ~/.ssh/id_rsa.pub
```
![](https://i.imgur.com/vLMuHSt.png1)

- **Step # 11:**  Now it will show you the ssh key. Just simply copy it.

![](https://i.imgur.com/vLMuHSt.png)

- **Step # 12:**  And now let’s head back to the github SSH key page and paste the key to the key field, press add ssh key. And done!

[![Add new SSH Key](https://i.imgur.com/AVUwPUQ.png "Add new SSH Key")](https://github.com/settings/ssh/new "Add new SSH Key")


Working with Remote Repositories
======================
- Go to your local directory and open git bash there.
- So let’s copy the code on git’s website which looks like this `git remote add origin https://github.com/yourusername/repositoryname.git` **(Repository Link)** and paste it to the git bash and press enter.

```shell
git remote add origin https://github.com/basitaminbhatti/Git-For-Beginners.git
```

![](https://i.imgur.com/nCdaqwa.png)


- Now we will paste the second command which pushes the files onto the remote server which is `git push -u origin master`

```shell
git push -u origin master
```
![](https://i.imgur.com/1JRzAdc.png)

- It will run and push your files to github.

![](https://i.imgur.com/2QgBcHl.png)

Alias
===
Alias is a term which is associated with shortcuts in Git. It shortens the long commands to increase efficiency. So let’s see how to set up an alias.
### Setting Up Alias:
- Open git bash and now type this command to set up alias for `git status`
- Type `git config --global alias.st status` and press enter.

```shell
git config --global alias.st status
```
![](https://i.imgur.com/zeJTdd3.png)

- Now what it means is if we type `git st` it will give us the output of `git status`

```shell
git st
```

![](https://i.imgur.com/czL5t0p.png)

- **Let’s do another one. **
- Now type `git config --global alias.unstage ‘restore --staged --’ `

```shell
git config --global alias.unstage 'restore --staged --' 
```
![](https://i.imgur.com/Atrcejp.png)

- Now if you type `git unstage` it will work as `git restore --staged --`

```shell
git unstage file.log
```

![](https://i.imgur.com/tjGusvO.png)

- We can set up as many aliases we want. Like we can create an alias for seeing the last commit done by the user.
- To do that type `git config --global alias.last 'log -p -1' `

```shell
git config --global alias.last 'log -p -1'

```
![](https://i.imgur.com/JrXyQ9r.png)


- Now if we type `git last` it will show us the last commit done by the user.

```shell
git last
```
![](https://i.imgur.com/ryuPTNj.png)

Creating & Switching Branches
====

### Branch:
Branch is a way to add new features or modification to the software and not affecting the main part of the project. We can also say that branches create another line of development in the project.

### Creating Branches:
- Master Branch 

![](https://i.imgur.com/rndPcDL.png)

- Open Git Bash on your local repository.
- Let’s create a branch by typing `git checkout -b branchname`

```shell
git checkout -b branchname
```
![](https://i.imgur.com/51icE7z.png)

- Now if you modify the files in the repo and do `git status` it will show you “on Branch branchname” which means you are changing files on the branch you have created.

```shell
git status
```
![](https://i.imgur.com/Uo5O956.png)

- Now change some file in **new idea** branch.

![](https://i.imgur.com/ASxAtB5.png)

- Let’s stage these files by using `git add .` and commit these changes by typing `git commit -m “commit message” `

```shell
git add .
git commit -m “commit message”
```
![](https://i.imgur.com/mKB49ZT.png)

### Switching Branches:

- Now if you do `git checkout master` then you will see that the files on your repo will revert to the master branch where we haven’t made any changes.

```shell
git checkout master
```
![](https://i.imgur.com/mkPkjff.png)

![](https://i.imgur.com/rndPcDL.png)

- Now if we do `git checkout branchname` we will switch from master branch to our newly created branch where we have modified files.

```shell
git checkout branchname
```
![](https://i.imgur.com/xXKdPsx.png)

![](https://i.imgur.com/ASxAtB5.png)

### Checking Branches:
- If you want to know how many branches are existing just run this command: `git branch`

```shell
git branch
```
![](https://i.imgur.com/SAfQfl9.png)

### Rename Branch:
- If you want to rename the current branch, you can do: `git branch -m <newname>`

```shell
git branch -m <newname>
```

![](https://i.imgur.com/mtlEPs7.png)

- If you want to rename a branch while pointed to any branch, do: `git branch -m <oldname> <newname>`

```shell
git branch -m <oldname> <newname>
```

![](https://i.imgur.com/cwjnJUI.png)


### Merge Branches:
- Now if we do `git merge branchname` it will merge those branches.

```shell
git merge branchname
```
![](https://i.imgur.com/zpmkeuJ.png)


### Merge Conflicts:
#### When Merge Conflicts happen?
When you merge branches that have competing commits, and Git cannot decide which changes to incorporate in the final merge, that's when merge conflicts happen.

#### Resolving Conflicts:
There are many ways to resolve conflicts on Git Merge. But we are going to use the easiest one. By using VSCode. [Just Install VS Code](https://code.visualstudio.com/download "Just Install VS Code") in your system and open those files who have conflicts, and you will see 2 options: **Current Change** and **Incoming Change**. Just like this.

![](https://i.imgur.com/NyI5gSe.png)

Just choose **Accept Incoming Change**. Save the file and commit the files by typing `git add .` and`git commit -m “message”` Now you have successfully merged 2 branches.


### Deleting Branch:
- Delete the specified branch. This is a **“safe”** operation in that Git prevents you from deleting the branch if it has unmerged changes.

```shell
git branch -d <branch>
```
![](https://i.imgur.com/kiEF07U.png)

- Force delete the specified branch, even if it has unmerged changes. This is the command to use if you want to permanently throw away all of the commits associated with a particular line of development.

```shell
git branch -D <branch>
```

![](https://i.imgur.com/2nMVlWo.png)
















