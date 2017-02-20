# Git for Beginner

This tutorial will make you acquaintance to Git commands for managing a remote repository.


### 1. Tutorial 1
#### 2. Adding an existing project to GitHub using the command line

##### Step 1: 

Create a new repository on GitHub. To avoid errors, do not initialize the new repository with README, license, or gitignore files. You can add these files after your project has been pushed to GitHub. 

Otherwise, if you have already created the repository with  README, license, or gitignore files then you just have to make a “git pull <remote> <branch>” before pushing your all files.
[i.e., git pull https://github.com/khadija-ashraf/HelloWorldSpringMVC.git  master] 

##### Step 2:

Open Terminal.

##### Step 3:

Change the current working directory to your local project.

##### Step 4: 

Initialize the local directory as a Git repository.
```ssh
$ git init
```

##### Step 5:


```ssh
# Add the files in your new local repository. This stages them for the first commit.
$ git add .
```
Adds the files in the local repository and stages them for commit. To unstage a file, use 'git reset HEAD YOUR-FILE'.
##### Step 6:

Commit the files that you've staged in your local repository.
```ssh
$ git commit -m "First commit"
# Commits the tracked changes and prepares them to be pushed to a remote repository. To remove this commit and modify the file, use 'git reset --soft HEAD~1' and commit and add the file again.
```
##### Step 7:

Get the remote repository URL. At the top of your GitHub repository's Quick Setup page, click to copy the remote repository URL. 

##### Step 8:

In Terminal, add the URL for the remote repository where your local repository will be pushed.
```ssh
$ git remote add origin <remote repository URL>
# Sets the new remote
```

Now verify the URL

```ssh
$ git remote -v
# Verifies the new remote URL
```

##### Step 9:

Pull any existing files from the repository if there is any with the command “git pull <remote> <branch>”

```ssh
$ git pull https://github.com/khadija-ashraf/HelloWorldSpringMVC.git  master
```

##### Step 10:

Push the changes in your local repository to GitHub.

```ssh
$ git push origin master
# Pushes the changes in your local repository up to the remote repository you specified as the origin
```
--------------------
Refs:

https://help.github.com/articles/adding-an-existing-project-to-github-using-the-command-line/ 

http://rogerdudler.github.io/git-guide/
