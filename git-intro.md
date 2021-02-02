# A Comprehensive Guide for Git

we are going to explain version control besides Git system.

## Version control
Version Control is a system that allows you to revisit various versions of a file or set of files by recording changes.

## Git 
Git is a DVCS that stores data in a file system made up of snapshots. Each time you save a changed version of your project — called commit — Git creates a snapshot of the file and stores a reference to it.

## git and the cloud 
github is a cloud for restoring the code into reposotories.
how to use the git besides github:

1. you need to create a repo in github and you can create a copy of it or an exciting repo by using clone command
`$ git clone [your repo URL]`

2. to track all the files in a repo use: `$ git add [file name]` or by using `$ git add .` to track all the changes in all files.

3. after staging your files, you need to commit these changes using: `$ git -m "your message"` and we use the message to tell what and why we do these changes.


4. now you should push changes to a remote repo(which you had cloned), for example: `$ git push origin main`
this command pushes all changes from local to the cloud.