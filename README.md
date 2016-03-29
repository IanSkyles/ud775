# How to Use Git and GitHub - ud775 -Reflections
This repo contains reflections from my course "How to Use Git and GitHub" offered by Udacity.

##What this course taught me
By completing this course, I gained familiarity with one of the most popular version
control platforms, Git. I learned how to more effectively share code with friends, 
colleagues, and future and current employers all via GitHub.

##Why I took this course and Course Summary
Effective use of version control is an important and useful skill for any developer working on long-lived (or even medium-lived) projects, especially if more than one developer is involved. This course, built with input from GitHub, introduced the basics of using version control by focusing on a particular version control system called Git and a collaboration platform called GitHub.

##Why I took this course
Git is used by many tech companies, and a public GitHub profile serves as a great portfolio for any developer. But more than that, I wanted to establis an efficient programming workflow that allows me to:

* Keep track of multiple versions of a file
* Track bugs by reverting to previous working versions of a file
* Seamlessly collaborate with other developers on a project

The use of tools like Git and GitHub is essential for collaborating with other developers in most professional environments.

## Course Final Proect 
I published this repository containing my reflections from the course. Also, I forked a repo, made changes, merged the changes with two updates made in the master repo, then submitted a pull request (to collaborative Create-Your-Own-Adventure story).  

##Course Syllabus
###Lesson 1: Navigating a Commit History

In this lesson, I learned about a few different types of version control systems and discovered what makes Git a great version control system for programmers. I also got practice using Git to view the history of an existing project. I learned to see all the versions that have been saved, checkout a previous version, and compare two different versions.

###Lesson 2: Creating and Modifying a Repository

In this lesson, I learned how to create a repository and save versions of my project. I learned about the staging area, committing my code, branching, and merging, and how I can use these be more efficient and effective.

###Lesson 3: Using GitHub to Collaborate

In this lesson, I got practice using GitHub (remote repositories) to share my changes with others and collaborate on multi-developer projects. I learned how to make and review a pull request on GitHub. Finally, I got practice with all of the skills I learned in the course by collaborating with other Udacity students to write a create-your-own-adventure story.

##Definitions
###Staging Area : an area where you have added but not commited yet. Files waiting to be commited.
###Working Directory : the directory you are in. This stage comes before the staging area.

##Cheat Sheet

###Push deleted files to github from local repo.
```
git add . -A
git commit -m "Deleted some files..."
git push origin master
```
###Initialize a repository locally (creates a .git hidden file)
`git init`
###Add a file to the staging area
`git add fileNameHere`
###Check repository and file statuses
`git status`
###Remove a file from the staging area, that you accidentally added to the staging area.
`git reset fileNameHere`
###see the changes between the staging area and your working directory!
`git diff `
###	git diff --staged allows you to see the changes between the repository (most recent commit) and the staging area
`git diff --staged`
###Delete a branch
`git branch -d branchNameHere`
###Show differences between commit id and its parent
`git show commitIDHERE`
###Create a new branch and check it out
`git checkout -b new_branch_name`
This is the same as running
```
git branch new_branch_name
git checkout new_branch_name
```

###Merge Conflicts Locally
* top sections is your code (yourBranch)
* middle is original (common parent)
* bottom is their code. (master)
```
	git checkout yourBranch
	git merge master yourBranch 
```
###Recursively find a bug
```
git log
	git checkout previousVersionId 
```
		if no bug then it was introduced in the commit after it (previously checkedout)
		if a bug still exists
```
			git log
			git checkout previousVersionId
```
###Compare two commits, printing each line that is present in one commit but not the other.
`git diff id1 id2` will do this. It takes two arguments - the two commit ids to compare. 
###Make a copy of an entire Git repository, including the history, onto your own computer.
`git clone htttpsOfRepo` will do this. It takes one argument - the url of the repository to copy. 
###Temporarily reset all files in a directory to their state at the time of a specific commit.
`git checkout commitId` will do this. It takes one argument - the commit ID to restore. 
###Show the commits made in this repository, starting with the most recent. q to quit viewing git log.
`git log` will do this. It doesn't take any arguments.
###To see the version of git you have
`git --version`
	
