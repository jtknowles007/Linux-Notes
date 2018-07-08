# GIT Notes

## 12/10/2017

* Basic push to GitHub
    + git add to add <file> to update what will be committed
    + git add* to add all files that were touched for commit
    + can also use git commit -a to do the same
    + combine add and commit message by using git commit -a -m "your message here"
    + git push - will be asked for username and password
    + It appears that the benefit of specifically naming each file with add <filename> then committing individually is that you can give each committed file a specific commit comment.  If this is not important - if all files committed can have the same comment - you can use the add* and commit -m OR git commit -a -m "your message here" to take care of it all in one fell swoop.
* Basic pull from GitHub
    + git pull downloads history and incorporates changes from master to the local copy of the repository. This command combines the fetch and merge commands into one action.  These two can be run separately
