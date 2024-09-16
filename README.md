## Git Workshop - Git is a version control system 

- Create folder and initialize git to track files for version control using 

```
git init
```
- Check status of files using

```
git status
```

- Files in Git contains three stages : Untracked, Staged and Tracked

- Create a new file - untracked 

- Add files to be staged using

```
git add 'filename' or git add .
```

- Unstage a file

```
git rm --cached 'filename'
```

- Commit files to be tracked using

```
git commit -m "add message"
```

- Delete a file 

```
rm 'filename'
```

- Restore deleted file, if already commited(tracked) using

```
git restore 'filename'
```

- Check history of commands used

```
history
```

- Push changes onto the GitHub Repository, first create a new repository with the same name as the folder in git

```
git remote add origin 'http gitHub repo link'
git push -u origin main
```
above 2 commands will give an error probably -- "error: failed to push some refs to 'http gitHub repo link' "

- Eliminate this error by creating a Personal access token from developer settings, give Note, Expiration  and  Select scopes(as per choice, ex. 7 days)and then copy access token to use in next command

- Change the remote URL to your new repository, if the current remote is still pointing to the old repository, update it to the new one. :

```
remote set-url origin http://accesstoken@github.com/ritikasharma1505/GitHub-For-DevOps-Workshop.git
```

- Check your current remote

```
git remote -v
```

- Push the code to the new repository: Now that your remote is updated, you can push your code to the new repository:

```
git push origin master
```
- fatal: The current branch master has no upstream branch. To push the current branch and set the remote as upstream, use

```
git push --set-upstream origin master
```

- Clone or make a copy of a remote repository(GitHub) to your local repository(Git)

```
git clone 'http repo link'
```

- Bring the code from remote(GitHub) to local machine(Git)

```
git pull origin master  or git pull
```

- Branches in Git and GitHub, Every branch maintain its own copy, Create a new branch and switches you to that branch

```
git checkout -B 'branchname'  
```
- Create a new branch without switching to that branch (only creates)

```
git branch 'branchname'
```
- Check branches created or available

```
git branch
```
- Switch to other branch

```
git switch 'branchname' or git checkout 'branchname'
```
- Check one line logs, HEAD represents the latest commit

```
git log --oneline
```
