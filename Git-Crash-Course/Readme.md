## Git Hidden Folder

There is a hidden folder called `.git` which tells you that our project is a git repo.

If we wanted to create a git repo in a new project, we create the folder and initialize that folder using `git init`

```
mkdir /workspaces/tmp/new-project
cd /workspaces/tmp/new-project
git init
touch Readme.md
code Readme.md
# make changes to file
git commit -a -m "add readme file

```

## Cloning

We can clone 3 ways: HTTPS, SSH and Github CLI

### HTTPS

```
git clone HTTPS address in code 
```

> To do this, you will need to generate a Personal Access Token (PAT)
https://github.com/settings/tokens?type=beta


You will use the PAT is a password when logging in when trying to to push to the remote

### SSH

```
git clone SSH address in Code
cd GitHub-Examples
```

We will need to creat our own SSH rsa key pair

```
ssh-keygen -t rsa
```

We can test our connection here:
```
ssh -T git@github.com
```

For WSL users and if you create a non default key you might need to add it.

Have to look into how to change account via terminal

### Github CLI



## Commits

When you want to commit a change, use `git commit`

```
git commit -m "notes on commit"
```

If you don't use -m, you will open a txt file and have to enter what changes you are making.  With -m you can just enter the txt of why you are making the commit

On a local machine, you can enter the global information for committing:

```
git config --global core.editor emacs
```

## Branches
## Remotes
## Stashing
## Merging

## Add

When we want to add all the files that we have made changes too

```
git add .
```

## Reset

Reset allows you to remove files that you have committed

```
git reset
```

## Status

Tells you what files will or will not be committed

```
git status
```

## Gitconfig File

The gitconfig file is what stores your global configuartions for git such as email, name, editor and more.

Show the contents of our git config file
```
git config --list
```

When you first install Git on a machine you are supposed to set up your name and email

```
git config --global user.name "John Doe"
git config --global user.email "John@doe.ca"
```

## Log

git log will show recent commits to the git tree

```
git log
```

## Push

When we want to push a repo to our remote we push

```
git push
```