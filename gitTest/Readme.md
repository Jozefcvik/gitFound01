## GIT hidden folder

There si a hidden folder called `.git `

If we wanted to create a git repo in a new project we' created the folder and the initialize that repo using `git init`

```
mkdir /workspaces/tmp/new-project
cd /workspaces/tmp/new-project
git init
touch Readme.md
open Readme.md
git status
#makes changes to readme.md
git commit -a -m "add README file"
```

## Cloning

We can clone three ways: HTTPS, SSH, Github CLI

Since we are using GitHub Codespace we´ll create a temporary directory in our workspace

```sh
mkdir /workspace/tmp
cd /workspace/tmp
```

### HTTPS

```sh
git clone https://github.com/...
```


## Commits

when we want to commit code we can write git commit which will open up the commmit edit message in the editor of choice.

```sh
git commit 
```

Set the global editor
```
git config --global core.editor nano
```


## Branches

## Remotes

## Stashing

## Merging

## Add

```
git add Readme.md
git add .
```

## Reset

Reset allows you to move Staged changes to be unstaged.
This is useful when you to revert all files not to be not commited

```
git add .
git reset
```

> git reset will revert a git add.

## Status

Git status show you what files will or will not be commited.

```
git status
```

## Gitconfig file

The gitconfig file is what stores your global configurations for git such as email, name, editor and more.

showing the contents of our .gitconfig file
```
git config --list
```

When you first install Git on a machine you are suppose to set up your name and email

```sh
git config --global user.name "John Doe"
git config --global user.email "johndoe@example.com"
```

## Log

git log will show recent git commits to the git tree


## Push

When we want to push a repo to our remote origin

```
git push origin main
```
