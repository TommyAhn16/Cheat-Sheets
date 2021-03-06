# Git Command Cheat Sheet

Referenced Github document from [here](https://training.github.com/downloads/github-git-cheat-sheet/)

## 1. Create repositories

### Make new git repo

```shell
$ git init
```

- Turns an existing directory into a new Git repository inside the folder you are running this command.

### Add remote gihub repo to local

```shell
$ git remote add origin [url]
```

- Specifies the remote repository for your local repository. The url points to a repository on GitHub.

### Clone repo

```shell
$ git clone [url]
```

- Clone (download) a repository that already exists on GitHub, including all of the files, branches, and commits

## 2. Branches

Any commits you make will be made on the branch you’re currently “checked out” to.

### Rename branch

```shell
$ git -M [new name]
```

### Branch status

```shell
$ git status
```

- Return status of the current branch, including which branch I am in

### Make new branch

```shell
$ git branch [branch-name]
```

- Creates a new branch

### Switch working branch

```shell
$ git checkout [branch-name]
```

- Switches to the specified branch and updates the working directory

### Make new branch and switch

```shell
$ git checkout -b [new branch-name]
```

- Makes new branch and checks out to the new branch

### Delete branch

```shell
$ git branch -d [branch-name]
```

- Deletes the specified branch

### Delete remote branch

```shell
$ git push origin --delete <branch>
```

### Delete a local remote-tracking branch

```shell
$ git branch -dr <remote>/<branch>
```

## 3. Make changes

### Add all changes

```shell
$ git add .
```

### Adds specific file

```shell
$ git add [file]
```

### Commit

```shell
$ git commit -m "[descriptive message]"
```

## 4. Synchronize changes

### Setup upstream and push

```shell
$ git push -u [upstream branch] [local branch]
```

### Upload changes to github

```shell
$ git push -u origin main
$ git push
```

### Pull

```shell
$ git pull
```

- Updates current local working branch with all new commits from the corresponding remote branch on GitHub. git pull is a combination of git fetch and git merge
