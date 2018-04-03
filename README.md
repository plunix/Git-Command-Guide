# Git Command Guide

<h1 align="center">
	<br>
	<br>
	<img  src="https://cdn-images-1.medium.com/max/800/1*BCZkmZR1_YzDZy22Vn4uUw.png" alt="git-germancutraro">
	<br>
	<br>
	<br>
</h1>

> Git is a version control software designed by Linus Torvalds, thinking about the efficiency and reliability of maintaining application versions when they have a large number of code files.

## Advantages:
  - ✔️ Better teamwork
  - ✔️ Control of changes in the project
  - ✔️ Audit and reliability
  - ✔️ Return to previous versions
  - ✔️ Local & Remotes Repositories
  - ▪️▪️▪️ And much more

> **Download** <br>
    Linux Debian: `$ sudo apt-get install git` <br>
    Linux Fedora: `$ sudo yum install git` <br>
    [Mac](http://git-scm.com/download/mac) <br>
    [Windows](http://git-scm.com/download/win) <br>
    **You can write the commands in your CMD or in the git bash terminal**

## About this Guide::
  - 🔈 Everything in bold means that the value is relative, it changes according to each one.
  - 🔈 Is not a finished version.

## Star the Project :star:

The _easiest_ way you can _contribute_ is
by "_starring_" this project on GitHub!
This will help you to "_bookmark_" the content so you can return to it.
But it will also help the people who "_follow_" you on GitHub to _discover_
that you find it _interesting_ or _useful_.

The _more_ people star and _share_ the project, the more possible contributors are able to understand the value of contributing and *open sourcing their knowledge*!

:octocat: I will be grateful that you follow me :octocat:

# Commands 🚀

___

### GIT Version: 🕵

```
git --version
```

### Set name credential: ✋

<pre>
git config --global user.name <b>"germancutraro"</b>
</pre>

### Set E-mail credential: ✉️

<pre>
git config — global user.email <b>“germancutraro@hotmail.com”</b>
</pre>

### Help Command 🙏

```
git help  
```

### Get help from a specific command 👏

<pre>
git help <b>commit</b>
</pre>

### Create a Repository 👊

<pre>
git init
</pre>

### Add a file 👉

<pre>
git add <b>index.html</b>
</pre>

### Add multiple files 🖖
<pre>
git add <b>index.html index.js</b>
</pre>

### Add all files 💥

<pre>
git add .
</pre>

### Add all the files in the current directory by their extension: 🌕

<pre>
git add <b>*.txt</b>
</pre>

### Add all the files that are in a folder: 📁

<pre>
git add <b>css/</b>
</pre>

### Add all the files that were modified: 〽️

<pre>
git add -u
</pre>

### Add all the files by their extension that are inside a folder: 📂

<pre>
git add <b>pdfs/*.pdf</b>
</pre>

### See modified files 🔦

<pre>
git status
</pre>

### See the modified files without so much information: 🤐

<pre>
git status -s
</pre>

### See the modified files and in which branch we are working: 🔆

<pre>
git status -sb
</pre>

### Delete a file that was in the staging area  ⛔️

<pre>
git reset <b>index.js</b>
</pre>

### Delete a file that was in the staging area by their extension ❌

<pre>
git reset <b>*.xml</b>
</pre>

### Commit Changes 📝

<pre>
git commit -m <b>'Add the navbar'</b>
</pre>

### See all the commits that we did 👀

<pre>
git log
</pre>

### See all the commits that we did in a pretty way 🌲

<pre>
git log --oneline --decorate --all --graph
</pre>

### Create a Aliase/Shortcut 💧

<pre>
git config --global alias.<b>lg</b> "log --oneline --decorate --all --graph"
</pre>
*So now we can do: `git lg` for the pretty log command* 👆

### To see the configuration file 📘

<pre>
git config --global -l
</pre>

___

## Review of the basic and important commands

- `$ git init` -> Initialize a local Git Repository
- `$ git add <file>` -> Add file to the Staging Area
- `$ git status` -> Check status of files in the working branch
- `$ git commit` -> Commit Changes
- `$ git push` -> Push to Remote Repository

<h1 align="center">
<img src="https://cdn-images-1.medium.com/max/1000/1*j-Hp4pn4NNx35nDP3qEniw.png" alt="git-germancutraro">
</h1>

### See all the changes that happened between the last commit and now 📍

<pre>
git diff
</pre>

### See all the files that are in the Staging Area ⭕

<pre>
git diff --staged
</pre>

### Recover Files 💞

<pre>
git checkout .
</pre>

### Delete all the changes added in a file 📄

<pre>
git checkout -- <b>README.md</b>
</pre>

### Add files and commit in the same command: 🌟

<pre>
git commit -am <b>'README actualizado'</b>
</pre>

### Edit the commit message ✏️

<pre>
git commit --amend -m <b>'We edited the message!'</b>
</pre>

### Add or Back to the last commit ↶

<pre>
git reset --soft HEAD^
</pre>

### Return to a specific commit in a weak way ↖️

<pre>
git reset --soft <b>39ae8e6</b>
</pre>

### Return to a specific commit in a hard way ⬅️

<pre>
git reset --hard <b>39ae8e6</b>
</pre>

### List of originated commits 📋

<pre>
git reflog
</pre>

### Go back to a point 🔄

<pre>
git reset --hard <b>43809d4</b>
</pre>

### Rename Files ✍️

<pre>
git mv <b>index.js app.js</b>
</pre>

### Delete Files ❌

<pre>
git rm <b>app.js</b>
</pre>

## Branches

> A branch is basically a new timeline that stores commits. They are used to develop functionalities independent of each other. The master branch is the default branch when you create a repository. Create new branches during development and merge them to the main branch when you finish.

<h1 align="center">
<img src="https://cdn-images-1.medium.com/max/800/1*j5j40VU7z5HYF7R31v-NFg.png" alt="git-germancutraro">
</h1>

### Create a branch: 🔱

<pre>
git branch <b>myBranch</b>
</pre>

### See the branches of our repository: 🔅

<pre>
git branch
</pre>

### Work in a specific branch 🌿

<pre>
git checkout <b>myBranch</b>
</pre>

### Create and move to a branch in a single command 🍀

<pre>
git checkout -b <b>myBranch</b>
</pre>

## Merge branches:

### First we go back to the master branch: ❄️

<pre>
git checkout master
</pre>

### And now we run the next command 🌻

<pre>
git merge <b>myBranch</b>
</pre>

### Once merged we can proceed to delete the branch 🌹

<pre>
git branch -d <b>myBranch</b>
</pre>

## Tags

### Create a tag 💅🏼

<pre>
git tag -a <b>v1.0.0</b> -m <b>"Version 1.0.0"</b>
</pre>

### Insert a tag in a specific commit 🔖

<pre>
git tag -a <b>v0.1.0 43809d4</b> -m <b>'Alpha Version'</b>
</pre>

### See all Tags 🎌

<pre>
git tag
</pre>

### See the tag message 👁‍🗨

<pre>
git show <b>v1.0.0</b>
</pre>

### Delete a tag ✖️

<pre>
git tag -d <b>v0.1.0</b>
</pre>

## Stash

### Creation 📦

<pre>
git stash
</pre>

### Get the list 💼

<pre>
git stash list
</pre>


# Github

<h1 align="center">
	<br>
	<br>
	<img  src="https://cdn-images-1.medium.com/max/800/1*sv-zoywuB4JsiHgVWZ3m8w.png" alt="github-germancutraro">
	<br>
	<br>
	<br>
</h1>

### Once we create a repository, we can add it to the remote server: 📮

<pre>
git remote add origin <b>yourRepo.git</b>
</pre>

### See the remote sources of our repository: ⬛

<pre>
git remove -v
</pre>

Once we have all our commits done and we have added the remote repository we can upload our files to Github:

### Push: ✈️

<pre>
git push -u origin master
</pre>

<h1 align="center">
<img src="https://cdn-images-1.medium.com/max/1000/1*j-Hp4pn4NNx35nDP3qEniw.png" alt="git-germancutraro">
</h1>

But, as you can see, the tags are not uploaded with the `git push` command:

<h1 align="center">
<img src="https://cdn-images-1.medium.com/max/800/1*OL18-Je8x7ODLRatLatJgA.png" alt="git-germancutraro">
</h1>

### Push the tags ▶️

<pre>
git push --tags
</pre>

### Ignore Files ❗️

<sub>For this, you must create a .gitignore files, and there you can write the files and foulders that you dont want to upload to the github repository like:</sub>

<pre>
node_modules
package-lock.json
</pre>

### Pull 🌌

<pre>
git pull
</pre>

<h1 align="center">
<img src="https://cdn-images-1.medium.com/max/1000/1*8QCb7E9u2xaQn2AEeAr-Jg.png" alt="git-germancutraro">
</h1>

### Clone a Repository ⌛

<pre>
git clone <b>repoUrl.git</b>
</pre>

### Clone a repository in a specific folder 📁

<pre>
git clone <b>repoUrl.git my-folder</b>
</pre>

___
### git undo
This will unstage all files you might have staged with git add:

git reset
This will revert all local uncommitted changes (should be executed in repo root):

git checkout .
You can also revert uncommitted changes only to particular file or directory:

git checkout [some_dir|file.txt]
Yet another way to revert all uncommitted changes (longer to type, but works from any subdirectory):

git reset --hard HEAD
This will remove all local untracked files, so only git tracked files remain:

git clean -fdx
WARNING: -x will also remove all ignored files!


But then after a while things started to get complicated. I had to work with submodules, change the remote URL, and handle untracked files. That is when I decided to move out of my comfort zone in Visual Studio and into the Git CLI.
The Git CLI is not easily remembered and everything can be done in more than one way so I started my own compilation of useful commands. Below is the result of that compilation. I hope it can be useful for those of you going through the same process and please let me know if you have any Git gems of your own that belong on the list.
The list
In no specific order whatsoever.
Edit configuration
On Windows the Git configuration file is usually placed under “c:\Users[user]”. You can also start an editor from the command prompt.
git config --global -e
Set editor for commit messages
To change the default editor for commit messages to Notepad++, add a [core] section to the config file looking like this.
[core]
    editor = 'C:/put-your-folder-here/Notepad++/notepad++.exe' -multiInst -notabbar
From now on Notepad++ will open when ever you run git commit without the -m switch.
Set merge tool to Visual Studio
[diff]
    tool = vsdiffmerge
[difftool]
    prompt = true
[difftool "vsdiffmerge"]
    cmd = \"C:\\Program Files (x86)\\Microsoft Visual Studio\\2017\\Professional\\Common7\\IDE\\CommonExtensions\\Microsoft\\TeamFoundation\\Team Explorer\\vsDiffMerge.exe\" \"$LOCAL\" \"$REMOTE\" //t
    keepbackup = false
    trustexistcode = true
[merge]
    tool = vsdiffmerge
[mergetool]
    prompt = true
[mergetool "vsdiffmerge"]
    cmd = \"C:\\Program Files (x86)\\Microsoft Visual Studio\\2017\\Professional\\Common7\\IDE\\CommonExtensions\\Microsoft\\TeamFoundation\\Team Explorer\\vsDiffMerge.exe\" \"$REMOTE\" \"$LOCAL\" \"$BASE\" \"$MERGED\" //m
    keepbackup = false
    trustexistcode = true
Submodules
Cloning submodules
If the repo contains submodules, and you want to bring the code in the submodules down, you’ll need to clone recursively.
git clone --recursive https://github.com/hocuspocus/icsharp.git
Change submodule to own fork
If you have cloned a repo with a submodule and you want to change the submodule to a different fork (if for example you have forked the submodule), you need to edit the URL in the file .gitsubmodule.
[submodule "Engine"]
    path = Engine
    url = https://github.com/scriptcs/scriptcs.git
After saving .gitsubmodule, run the command.
git submodule sync
It seems that this may detach from HEAD, so a checkout may be necessary (before making any local changes).
git checkout
If you have trouble downloading the code for the submodule, try running the command:
git submodule update --remote
Start merge tool
If there is a merge tool, you can start your merge tool (set in the config file).
git mergetool
Compare to remote
Start by fetching all from the remote repo:
git fetch origin
Then compare with local:
git log HEAD..origin/master --oneline
If you are happy with the results, you may merge the remote changes with the local repo:
git merge
Show remote URL
Show remote URL for “origin”:
git remote get-url origin
For a bit more information you may use:
git remote show origin
I your remote has moved, you can change the URL using set-url:
git remote set-url origin https://hocuspocus@bitbucket.org/myteam/myproject.git
Delete branch
Delete the remote branch:
git push -d <remote_name> <branch_name>
For example:
git push -d origin my-feature-branch
You may also use:
git push <remote_name> :<branch_name>
Delete the local branch:
git branch -d <branch_name>
Delete local changes
Undo all unstaged local changes:
git checkout .
Undo git add for at single file:
git reset folder/file.cs
Undo git add . :
git reset .
Fix untracked files
git rm . -r --cached
git add .
git commit -m "Fixed untracked files"
