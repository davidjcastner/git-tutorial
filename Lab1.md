# Lab 1 - Creating a repository and making the first commit

>**What is Repository?**  
Repository is commonly referred to as a “repo”.  
A repository is a project’s folder/directory.  
It stores the commits of a project as a series of referenced objects called HEADs.  
There are two versions of GitHub repos, public and private. Public ones are free, and you have to pay for private ones.  
The name, “username/organization.github.io”, is reserved repo for the user or organization GitHub page (website).

## Commands used in this lab

**git clone _url_** - clones a remote repository to your local machine  
**git add _files_** - adds changes that you made to the staging area  
**git commit -m _“commit message”_** - commits all staged work and provides a short message about the committed work


### Step One

Create a repository on the website. Name the repository `git-tutorial`, and select the option to **Initialize this repository with a README**. The rest of the options can be left blank.

### Step Two
-m
Clone the repository to your local machine. To do this: open up the terminal or git shell and navigate to where you want the repository to be stored. To navigate in the terminal the command `cd path/to/directory/` can be used. Looking up a cheat sheet or basic tutorial for command line may be useful if you are not familiar with it.

Once you have navigated to the location you want the repository to be stored, clone the repository with the command `git clone https://github.com/username/git-tutorial.git` or `git clone git@github.com:username/git-tutorial.git` **inserting your own _username_**. You can copy the url address from the GitHub website as well. If you are using the windows git shell that came with the desktop, you will most likely be using the ssh url. Cloning the repository makes a copy of the repository on your local machine. The repository will be a folder on your computer that you can navigate to in any file explorer.

### Step Three

Create a file called `languages.txt` in the repository. This can be done by opening up the location of the repository in a file explorer, right click and select new text file. You can edit this file in your favorite text editor.

In this file, add all of the programming languages that you know. If you don't know any programming languages add a couple that you would like to learn.

**Example:** `path/to/repo/languages.txt`

```
python
javascript
c++
```

Once you have added all of the files, save the file.

### Step Four

Navigate to the location of your repository in the terminal or git shell. If you are using the same terminal as before, the command should be `cd git-tutorial`.

Verify that you have added and saved the file `languages.txt` to the right location with the command `git status`. You should see that the file is currently untracked:

```
On branch master
Your branch is up-to-date with 'origin/master'.
Untracked files:
  (use "git add <file>..." to include in what will be committed)

	languages.txt

nothing added to commit but untracked files present (use "git add" to track)
```

Having untracked files means that they will not be included in the repository.

Add the file to the staging area with the command `git add languages.txt`. The staging area keeps track of all the changes that you will add to the repository in the form a commit which is the next step. This allows you select which changes you want to add without removing other work that you have done.

Using the command, `git status`, again will show that languages.txt has been added to the staging area:

```
On branch master
Your branch is up-to-date with 'origin/master'.
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

	new file:   languages.txt

```

### Step Five

Next you can commit the changes in the staging area to repository with the command `git commit -m "add languages"`. The `-m` option for the commit command allows for a message to attached to the work that was done. This message is very useful for tracking what changes were done.

The file languages.txt is now included in your local repository. The next lab will cover uploading it to the remote repository on GitHub.

**Lab 1 complete: Congratulations you have made your first repository and commit!**

Next lab:
**[Lab 2: Understanding remote and local work](Lab2.md)**

[Return to main page](/)
