---
layout: post
title:  "Lecture#1: Missing Semester"
date:   2020-07-01 16:16:45 +0800
categories: blog-post
---

# Missing Semester IAP 2020

Computers are very powerful. But without the right tool, we won't be able to maximize its capacities. This course teaches a vast range of tools available that makes us more efficient in dealing with computer-related problems. 

This blog post is part of my LecturesDuringQuarantine Series. I wrote this while watching the lecture videos (video and lecture links are provided). I only watched videos I think I will use in the future so I'm skipping some. 

**[Lecture 1: Shell using Bourne Again Shell](https://missing.csail.mit.edu/2020/course-shell/)**



* `<date>` - shows you time and date
* `<echo>` - results the string after ‘echo’
* `<echo $PATH>` - lists all the paths of the computer
* `<which echo>` - results the path that runs ‘echo’
* Directories
  * `<pwd>` - print working directory
  * `<cd>` -change directory
  * `<.>` - current directory
  * `<..>` - parent directory
  * `<ls>` - list files in the directory
  * `<ls ..>` - list files in a specified directory
  * `<cd ~>` - goes to your home directory
  * `<cd - >` - goes to directory you’re previously in 
* `<ls --help>` - list of information about the FILEs
* `<ls -l>` - gives more information about the files (group owner)
  * Read `<ls>` - are you allowed to see which files are in this directory
  * Write - are you allowed to rename, create, remove files in this directory
  * Execute `<search>` - are you allowed to enter this directory
* Changing directories
  * `<mv (path from) (path to)>` - move files
  * `<cp>` - copy the file 
  * `<rm>` - remove file
  * `<rmdir>` - remove a directory if its empty
  * `<mkdir>` - make a new directory, use quotation marks
* `<man ls>` - manual page for ls
* Crtl + l - clear
* Making a File with content
  * '<' - rewire the input of this program to be the context
  * '>' rewire the output of the preceding program into this file
* | - pipe, take the output of the program to the left and make it the input of the program to the right
* <tail> - last n lines of the input
* Root User
  * User id 0 
  * Allowed to do whatever they want 
  * `<sudo>` - super user do 
  * `<sudo su>` - for you to be the administrator

**[Lecture 2: Shell Tools and Scripting](https://missing.csail.mit.edu/2020/shell-tools/)**
* `<grep>` - search  in a file 
* `<echo $(pwd)>` - results the current directory
* `<ls *.sh>` - outputs all files with .sh extension
* `<convert image.png image.jpg>` - converts images
* `<vim  script.py>`-  shows python script 
* `<man rg>` - 
* `<find . -path ‘**/test/*.py’ -type f>` - finds all path with .py file
* `<&&>` - and operator
* `<||>` - or operator
* `<;>` - always true 

**[Lecture 3: Editors (vim)](https://missing.csail.mit.edu/2020/editors/)**
* Learning a new editor:
  * Start with a tutorial
  * Stick with using the editor for all your text * editing needs
  * Look things up as you go
* Popular editions
  * Visual studio code
  * Vim - popular command-line-based editor
* Operating modes 
* Normal - moving around a file and making edits
  * `<o>` - creates a new line below and goes to insert mode
  * `<O>` creates a new line above
  * `<u>` - undo
  * `<c-r>` - redo (control R) 
  * `<dw>` - deletes a word
  * `<de>` - deletes end of the word
  * `<ce>` - change end of the word and goes to insert mode 
  * `<x>` - deletes that character 
  * `<r>` - replaces a character
* Insert - for inserting text `<i>`
  * Press `<esc>` to go back to normal mode
  * You can rebind `<esc>` on your keyboard 
  * `<c2w>` - change word
  * `</>` - search 
* Replace - for replacing text; press `<R>`
* Visual - for selecting blocks of text; press `<v>`
  * Line	
  * Block; press `<c-v>`
  * `<h><j><k><l>` - select a block of text
  * `<y>` - copy and goes to normal mode
  * `<p>` - paste
  * `<V>` - copy lines of text 
* Command-line - running a command; press <:>
  * `<quit>` - quits vim 
  * `<:w>` - writes on the file so you can ‘save’ it
  * `<:help :w>` - get help for a ‘w’
  * `<:qa>` - quit all
  * `<c-d>` -page down
  * `<c-u>` - page up
  * `<fc>` - find the first ‘c’ in text
* Customizing Vim
  * plain -text configuration file in ~/.vimrc
* Plug-ins
  * Ack.vim - code search
  * Nerdtree - file tree
  * Vim-easymotion - magic motions 

**[Lecture 6: Version Control (git)](https://missing.csail.mit.edu/2020/version-control/)**
* Root
  * Tree - folder
  * Blob - file
* In Git, history is a directed acyclic graph (DAG) which means that each snapshot in Git refers to a set of “parents”
* “Edits” in new commit history actually create entirely new commits
* A commit has parents, metadata, and the top-level tree
* Reference - pointers to commits and are mutable (can be updated to point to a new commit)
* Git repository - the data objects and references
* `<git help <command>>` - get help for a git command
* `<git log>` - shows a flattened log of history
* Branches
  * `<git checkout -b <name>>` - created a branch and switched to it
  * `<git branch>` - shows branches
  * `<git branch <name>>` - creates a branch 
  * `<git merge <revision>>` - merges into current branch
  * `<git mergetool>` - uses a fancy tool to help resolve merge conflicts
  * `<git rebase>` - rebase set of patches onto a new base
  * `<git stash>` - temporarily remove modification to working branch
* Undo a File
  * `<git commit --amend>` - edits a commit’s contents/message
  * `<git reset HEAD <file>>` - unstage a file
  * `<git checkout -- <file>>` - discard changes
* Git Remote
  * `<git remote>` - list remotes
  * `<git remote add <name> <url>>` - add a remote
  * `<git push <remote> <local branch>:<remote branch>` - send objects to remote, and update remote reference
  * `<git fetch>` - retrieve objects/references from a remote
  * `<git pull>` - same as git fetch; git merge
  * `<git clone>` download a repository from remote
* Personal Notes
  * Always update your local files
    * `<git checkout master>`
    * `<git fetch>`
    * `<git pull --rebase origin master`
    * `<git checkout -b <name of new branch>>`
  * Do some changes on the website
    * `<git status>`
    * `<git add .>`
    * `<git commit>`
      * Ctrl + x, y, enter
    * `<git status>`
    * `<git push origin <name of new branch>>`
  * Editing commit history
    * `<git stash>`
    * `<git rebase -i HEAD~2>` - changing the last 2 comments
    * Reword your commit
    * `<git fetch>`
    * `<git status>`
    * `<git log>`
      * Press Q
    * `<git push origin <name of branch> --force>`
    * `<git stash>`
    * `<git stash pop>`
  * Here’s a highly recommended reading: [Pro Git](https://git-scm.com/book/en/v2)



