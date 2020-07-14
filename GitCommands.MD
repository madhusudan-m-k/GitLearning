### To start a new git project
~~~
git init
git add
git commit
git push
~~~

### List the git config details

~~~
git config --list
~~~

### Get the status about the branch on the local
~~~
git status
~~~

### Get Help about commands
~~~
git <command> --help
e.g. git commit --help

git help command
e.g. git help command

~~~

### Clone a remote  repository
~~~
git clone <git repo url> .
~~~

### To remove files from staging area -
~~~
git reset <filename>
~~~

### To remove ALL files from staging area  -
~~~
git reset
~~~

### To get the status of committed, staged  data -
~~~
git status
~~~

### To stage a specif file
~~~
git add <filename>
~~~

### To stage all files
~~~
git add -A
~~~

### To check the log of the changes
~~~
git log
~~~

### List the information about the remote repository -
~~~
git remote -v
~~~

### List all the branches for the repository -
~~~
git branch -a
~~~

### To look a the changes/diff the changes made
~~~
git diff
~~~

### To pull all the changes from the remote repository
~~~
git pull origin master
origin - is the reference to the repo held remotely
master -  is the branch name (master being the default, one can specify the actual branch)
~~~

### To pus all the local changes to the remote repository
~~~
git push origin master
git push
~~~

### Create a new LOCAL branch
~~~
git branch <branch name>
e.g. git branch cm-light-filter
~~~

### To list all the branches
~~~
git branch
the listing will have a * against the branch which is currently being pointed to and is being worked on
~~~

### To change the reference to the new branch or a different banch
~~~
git checkout <branch name>
git checkout cm-light-filter
~~~

### To commit the new branch to remote repository
~~~
git push -u origin <branch name>
git push -u origin cm-light-filter

-u will automatically orient the local new branch to the point to the remote new branch
~~~

### To switch branch from local branch to master
~~~
git checkout master
~~~

### To see which all branches has been merged to master
~~~
git branch --merged
~~~

### To merge a branch to the master
~~~
- make sure your current repo is pointing to the master 
git checkout master
git merge <branch name>
git merge cm-light-filter
~~~

### Commit the merge to the master
~~~
git push origin master
~~~

### Delete a branch after merge from the *local* repo
~~~
git branch --merge (to verify if the branch is already listed as a merged branch)
git checkout master (reorient the local working branch to master)
git merge <branch name>
git push origin master
git branch --merge (to verify the merged branch is listed in the merged branch list0
git branch -d <branch name>
~~~

### To delete the remote branch after merge
~~~
git push origin --delete <branch name>
git branch -a
~~~


### Commit file to Git

~~~
git commit -m "commit message" 
~~~

### Fetch all branches from remote repo
~~~
git fetch
~~~

### Restore uncommit file 
~~~
git checkout filename
~~~

### Check if anything has changed on the local repo
~~~
git status
~~~

### Do change difference within the local repo and the working copy
~~~
git diff
~~~

### View git commit logs
~~~
git log
~~~

### Change the wrong git commmit message without changing the change history
~~~
git commit --amend -m "your new log message"
~~~