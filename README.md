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

#### Save User Name And Password
```
git config --global credential.helper store
```

##### Initialize Repository
```
git init
```

##### Connect to Remote Repository
```
git remote add origin <remote_repo_url>
```
Here, origin is an alias, it can be anything

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
git push origin <branch_name>
```

```
git push origin <branch_name> --force
```

```
git push -u origin <branch_name>
```

```
git push
```

##### Fast push
```
git add .
git commit -m "commit_message"
git push origin <branch_name>
```



## Stash
##### Stash Changes (When we make changes, but we want to take pull but can't commit the changes)
```
git stash
```

##### List all stashes
```
git stash list
```

##### Apply a stash
```
git stash apply
```
```
git stash pop
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

##### Undo Pull
```
git reset --hard
```

##### Clear Staging area, Go Back to a Specific Commit
```
git reset --hard <commit_id>
```
```
git reset --hard HEAD{id}
```
HEAD{0} => HEAD  
HEAD{1} => a commit before HEAD  
HEAD{2} => two commits before HEAD and, so on


##### Create a Git Ignore File
```
touch .gitignore
```

##### Add files to Git Ignore
```
echo "example.txt" >> .gitignore
```

*.exe ignores all executable files  
<folder_name> ignores a folder and its content  


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

#### Create a Local Branch from Remote Branch
```
git checkout -b <local-branch>  --track origin/<remote-branch>
```

##### Fetch down all the branches from remote
```
git fetch origin
```

##### Switch to a branch
```
git checkout <branch_name>
```

#### Swith to a branch which does not exist on local but on remote
```
git fetch origin
git checkout -b <branch-name> origin/<branch-name>
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