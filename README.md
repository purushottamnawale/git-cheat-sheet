##### Add User Name and Email
```
git config --global user.name "John Doe"
git config --global user.email "johndoe@email.com"
```
```
git config --list
```
```
git config user.name
git config user.email
```

##### Initialize Repository
```
git init
```

##### Connect to Remote Repository
```
git remote add origin <remote_repo_url>
```

##### Rename a git branch
```
git branch -m <new_name>
```

##### Pull all files from Remote Repository
```
git pull origin main
```

##### Add all files
```
git add .
```

##### Commit all files
```
git commit -m “message”
```

##### Push files or a branch
```
git push origin main
git push origin main –force
```

##### check for modified and new files
```
git status
```

##### show all commits history
```
git log
```

##### Create a Git Ignore File
```
touch .gitignore
```

##### Show a list of branches
```
git branch
```

##### Create a branch
```
git branch <branch_name>
```

##### Switch a branch
```
git checkout <branch_name>
```

##### Delete a branch
```
git branch -d <branch_name>
```

##### Merge a branch into current branch
```
git merge <branch_name>
```

##### Change Git Commit
```
GIT_COMMITTER_DATE="Sun 14 May 2023 20:19:19 IST" git commit --amend --no-edit --date "Sun 14 May 2023 20:19:19 IST"
git commit --amend --no-edit --date="Sun 14 May 2023 20:19:19 IST"
git commit --amend --no-edit --date="13 Jul 2023"
```

##### Clone a Repository
```
git clone <remote_repo_url>
```