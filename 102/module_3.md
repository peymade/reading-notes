# Module 3 Reading

## Understanding Git

### Version Control

* (LVCS) Local Version Control: one database on a hard disk that stores changes
* (CVCS) Centralized Version Control: A single server stores all changes, and is accessible to multiple clients. 
* (DVCS) Distributed Version Control: Contains multiple mirrored repositories, allowing for collaboration without risk of losing a lot of the data

### What is Git?

**Git = DVCS**

When one saves a version of a project, it is saved as a snapshot. Every change is tracked by Git. Once these changes are committed, they can likely always be recovered. 

### States

* Committed -> Data stored in local database
* Modified -> File has been changed but not committed to database
* Modified -> File's changes have been flagged to be committed

### Importing Existing Project into Git

Importing means taking an existing project or directory and adding it to Git so that changes are tracked. 

1. Switch to target project or directory using `cd`
1. Use the `git init` command
1. `git add *.c`
1. `git add LISENCE`
1. `git commit -m "any message"`

### Cloning

Cloning is helpful when one wants to make a copy to the local drive of an existing Git repository.  

* Use the `git clone` command with the url of the repo
* To change the name, add the new name after the url

### Local Repository Structure

There are three parts to the local repository:
1. Working directory (actual files)
1. Index (staging)
1. Head (most recent commit)

### Saving Changes

**Tracked**: modified, unmodified, or staged. A part of the most recent snapshot.  
**Untracked**: not in the last snapshot, and not in the staging area.

### File Status

The cycle goes from untracked -> unmodified -> modified -> staged.   
When changes are committed, a file goes from "staged" to "unmodified."

Use `git status` to check the status of a file (if it is untracked, staged, etc.)

### Tracking and Staging New File

1 file? `git add ____ (file name)`   
All files? `git add *`

#### Commit

To commit the changes after staging 1 or more files:

`git commit -m "message about changes"`

To commit a snapshot of all changes to tracked files in pwd.
`git commit -a` 

### Push

Push these changes to a remote repository:

`git push origin main`

### Overview of Process

* Add = git add ___
* Status = git status
* Commit = git commit -m "message"
* Status = git status
* Push = git push origin main


[Home](README.md)
