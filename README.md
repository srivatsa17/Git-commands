# Git-commands
## 1. Clone a repository
**Command**
```
$ git clone <repository url>
```
**Example**
```
$ git clone https://github.com/srivatsa17/Git-commands.git
```
## 2. Create new branch from an existing branch locally and remote
**Command**
```
$ git checkout -b <new branch> <existing branch>
$ git push <remote name> <new branch>
```
**Example**
```
$ git checkout -b development master
$ git push origin development
```
## 3. Delete a particular branch
**Command**
```
$ git push -d <remote name> <branch name>
$ git branch -d <branch name>
```
**Example**
```
$ git push -d origin development
$ git branch -d development
```
