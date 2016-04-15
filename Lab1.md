# Lab 1 - Creating a Repo and making the first commit

Commands used in this lab:

**git clone _url_** - clones a remote repository to your local machine  
**git add _files_** - adds changes that you made to the staging area  
**git commit -m _“commit message”_** - commits all staged work and provides a short message about the committed work


### Step One

Create a repository on the website. Name the repository `git-tutorial`, and select the option to **Initialize this repository with a README**. The rest of the options can be left blank.

### Step Two

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

Verify that you have added and saved the file `languages.txt` to the right location with the command `git status`
