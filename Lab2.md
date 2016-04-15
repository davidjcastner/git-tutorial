# Lab 2 - Understanding remote and local work

>**Local** refers to any work done on the machine you are working on.
**Remote** refers to the repository stored on GitHub.

## Commands used in this lab

**git remote -v** - displays the location of the remote repository  
**git fetch** - checks the remote repository and updates your .git file (hidden) about changes in the remote repository  
**git pull** - pulls any commits from the remote repository to your local repository (specific to your working branch)  
**git push** - pushes any local commits to the remote repository (specific to your branch)

### Step One

From lab 1 on the GitHub website, you will notice that your commit is not there. That is because all of the work that you did only occured on your local machine, and your commit need to be pushed to GitHub before they will show up remotely.

First verify that the remote location is set to your GitHub with the `git remote -v` command. It should display the same URL that you used to clone the repository in lab 1.

### Step Two

Next, push the commit that you made with `git push`. After pushing, you should be able to see the new file `languages.txt` in your GitHub repository on the website.

### Step Three

In order in demonstrate how to get changes from the remote repository, you will need to make a change to one of the files through the website.

Open up GitHub in your browser and go to your git-tutorial repository. Select the languages.txt file and then select the option to edit it. It will be a pencil icon in the upper right hand corner.

Add a line of text at the top of file. If you aren't creative, you can add `Look a change!` to the top of the file. After adding the text, commit the changes (green button at the bottom of the page). This makes a commit to the repository just like in lab 1, but through the web browser.

Your languages.txt file should now look like this:

```
Look a change!

python
javascript
c++
```

### Step Four

In the terminal or git shell, run the command `git status`. Notice how your machine thinks that it is still up to date.

Using the command `git fetch` will check the repository for any updates since the last you checked. If you run `git status` again, you will notice that your local machine recognizing that it is one commit behind:

```
On branch master
Your branch is behind 'origin/master' by 1 commit, and can be fast-forwarded.
  (use "git pull" to update your local branch)
nothing to commit, working directory clean
```

### Step Five

In order to get the changes from the remote repository onto your local machine, run the command `git pull`.

If you open up `languages.txt` in your text editor, you should see the line of text that you added.

The pull command actually did a merge as part of the process which will be covered in the next lab.

**Lab 2 complete: Congratulations you were able to push and pull commits!**

Next lab:
**[Lab 3: Creating branches and merging](Lab3.md)**

[Return to main page](https://github.com/davidjcastner/git-tutorial)
