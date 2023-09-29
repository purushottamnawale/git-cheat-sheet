# Git Cheat Sheet


## Setup
##### Add User Name and Email
```
git config --global user.name "johnsmith"
git config --global user.email "johnsmith01@email.com"
```

#### Repository Information
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
`Here, origin is an alias, it can be anything`

##### Check Remote URL
```
git remote -v
```

##### Change the remote URL
```
git remote set-url origin <remote_repo_url>
```

## Save and Update
##### Pull all files from Remote Repository
```
git pull origin main
```
##### Stage files
```
git add <file_name>
```

```
git add .
```
##### Unstage files
```
git reset <file_name>
```
```
git reset .
```
##### Commit all staged files
```
git commit -m “message”
```

##### Push files or a branch
```
git push origin main
```

```
git push origin main –force
```

```
git push -u origin main
```

```
git push
```

##### Fast push
```
git add .
git commit -m "commit_message"
git push origin main
```

## Inspect
##### Check for modified and new files
```
git status
```

##### Show all commits history
```
git log
```

```
git log --oneline
```

```
git log --stat
```

##### Go to a specific commit 
```
git checkout <commit_id>
```

##### Change Commit Message
```
git commit --amend -m "New commit message"
```


##### Revert back to current head
```
git switch –
```

##### Clear Staging area, rewrite the working tree from specified commit
```
git reset --hard <commit_id>
```
```
git reset --hard HEAD{id}
```
`HEAD{0} => HEAD`  
`HEAD{1} => a commit before HEAD`  
`HEAD{2} => two commits before HEAD and, so on`


##### Create a Git Ignore File
```
touch .gitignore
```

##### Add files to Git Ignore
```
echo "example.txt" >> .gitignore
```

`*.exe ignores all executable files`  
`<folder_name> ignores a folder and its content`  


## Branch
##### Show a list of branches
```
git branch
```

```
git branch --all
```

##### Create a branch
```
git branch <branch_name>
```

##### Fetch down all the branches from remote
```
git fetch origin
```

##### Switch a branch
```
git checkout <branch_name>
```

##### Rename a branch
```
git branch -m <new_name>
```

##### Delete a branch
```
git branch -d <branch_name>
```

##### Merge a branch into current branch
```
git merge <branch_name>
```

##### Download a Repository with main branch
```
git clone <remote_repo_url>
```

##### Download a Repository with specific branch
```
git clone -b <branch_name> <remote_repo_url>
```



## Add SSH Key
```
ssh-keygen -t ed25519 -C "your_email@example.com"
```

Enter for for file name, to set default file name
Enter for passphrase, to set no passphrase

```
eval "$(ssh-agent -s)"
```

```
ssh-add ~/.ssh/id_ed25519
```

```
cat ~/.ssh/id_ed25519.pub
```

Copy the content and add it into GitHub/GitLab -> Settings -> SSH and GPG keys -> New SSH key


##### Change Commit Date Time

```
git commit --amend --no-edit --date="Sun 14 May 2023 20:19:19 IST"
```

```
git commit --amend --no-edit --date="13 Jul 2023"
```
