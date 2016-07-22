# Creating a new R package in RStudio with version control

Unlike other projects with GitHub, it is often easier to create the package locally
then begin version control.


### R Steps

First navigate to the directory in which you want to create the package

```
setwd("C:/Users/Jeff/Google Drive/")
```

Next use devtools to create the folder for the package. This creates the necessary 
starting files like the `DESCRIPTION` and `NAMESPACE`.

```
devtools::create("newpackage")
```

### Shell Steps

The next steps are also on a [GitHub Help Page](https://help.github.com/articles/adding-an-existing-project-to-github-using-the-command-line/)

Go to GitHub and create a new repository, BUT WITHOUT THE README OR LICENSE.

In RStudio, click on Tools > Shell to open a shell terminal. Navigate to the package directory.

```
$ git init

$ git add .
$ git commit -m "First commit"
```

Grab the remote repository URL from GitHub, then verify the remote URL

```
$ git remote add origin remote repository

$ git remote -v
```

Finally, push the changes to the repository
```
$ git push origin master
```






