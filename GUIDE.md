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
