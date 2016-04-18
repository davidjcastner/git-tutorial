# Lab 3 - Creating branches and merging

>**What are Branches?**  
Branches allow someone to work on a project without changing existing code.  
Example: You have a project with a working website. If you want to add a new feature to the website, you would create a branch which is a replica of the project for you to work with.  
A good practice is to keep the master branch as a working version of the software, and create a branch for developing individual features.  
The following branch names are reserved: “master” and “gh-pages”. “gh-pages” is a branch for a project’s GitHub page (website). "master"  is the default branch of a repository.  

>Below is an visual to illustrate branches where each node is a commit.  
<img src="https://blog.seibert-media.net/wp-content/uploads/2015/07/Git-Branches-1.png" style="padding:16px; border-radius: 20px; max-width:600px;" />


## Commands used in this lab

**git branch** - lists all branches on local machine and shows what is the current working branch  
**git checkout -b _branchname_** - creates a new branch with the specified branch name using the current branch as the base  
**git checkout _branchname_** - switches to the specified branch, work that is not committed with not be saved  
**git merge _branchname_** - merges the specified branch into the current working branch, merges are one-way operations

### Step One
