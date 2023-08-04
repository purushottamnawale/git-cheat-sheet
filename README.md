# Git Cheat Sheet

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

##### Check the remote URL

```
git remote -v
```

##### Change the remote URL

```
git remote set-url origin <remote_repo_url>
```

##### Pull all files from Remote Repository

```
git pull origin main
```

##### Add all files

```
git add <file_name>
```

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

##### check for modified and new files

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


##### Revert back to current head
```
git switch –
```


##### Create a Git Ignore File

```
touch .gitignore
```

## Branch

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

##### Rename a git branch

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


##### Change Git Commit Message
```
git commit --amend -m "New commit message"
```

##### Change Git Commit

```
git commit --amend --no-edit --date="Sun 14 May 2023 20:19:19 IST"
```

```
git commit --amend --no-edit --date="13 Jul 2023"
```
