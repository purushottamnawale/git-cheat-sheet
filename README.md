##### Add Name and Email
```
git config --global user.name "John Doe"
git config --global user.email "johndoe@email.com"
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
git branch -m <newname>
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
git commit -m “commit”
```

##### Push a branch
```
git push origin main
git push origin main –force
```

##### Create a Git Ignore File
```
touch .gitignore
```

##### Delete a branch
```
git branch -d <branch>
```

##### Change Git Commit
```
GIT_COMMITTER_DATE="Sun 14 May 2023 20:19:19 IST" git commit --amend --no-edit --date "Sun 14 May 2023 20:19:19 IST"
```