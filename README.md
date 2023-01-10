# Git commands
## 1. Configure username and email
**Command**
```
$ git config --global user.name "<username>"
$ git config --global user.email <email id>
```
**Example**
```
$ git config --global user.name "John Doe"
$ git config --global user.email johndoe@example.com
```
## 2. Create a new local repository
**Command**
```
$ git init
```
> Note: Create a folder in your system and run this command to create a local repository.

## 3. Clone a repository
**Command**
```
$ git clone <repository url>
```
**Example**
```
$ git clone https://github.com/srivatsa17/Git-commands.git
```
## 4. Create a new branch, switch to it and push to remote
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
## 5. Switch from one branch to another
**Command**
```
$ git checkout <existing branch>
```
**Example**
```
$ git checkout development
```
## 6. List current branch
**Command**
```
$ git branch
```
## 7. List all branches
**Command**
```
$ git branch -a
```
## 8. Push all local branches to remote
**Command**
```
$ git push -all <remote name>
```
**Example**
```
$ git push -all origin 
```
## 9. Delete a particular branch from remote and local
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
## 10. Adding a changed file to staging
**Command**
```
$ git add <filename>
```
**Example**
```
$ git add README.md
```
## 11. Adding multiple changed files to staging
**Command**
```
$ git add *
```
## 12. Commit changes to head but not to remote
**Command**
```
$ git commit -m "Commit message"
```
**Example**
```
$ git commit -m "First commit"
```
## 13. Push changes to remote
**Command**
```
$ git push <remote name> <branch name>
```
**Example**
```
$ git commit origin master
```
> Note: If upstream branch is already configured, just run `$ git push`

## 14. Get status of changed files
**Command**
```
$ git status
```
## 15. Fetch and merge changes on the remote server to your working directory
**Command**
```
$ git pull
```
## 16. Merge a branch into current branch
**Command**
```
$ git merge <branch name>
```
**Example**
```
$ git merge development
```
> If current branch is master, this will merge branch development into master.

## 17. See the difference between previous and current versions of file modified
**Command**
```
$ git diff
```
## 18. Reset/Undo the files modified to its previous version
**Command**
```
$ git reset
```
## 19. Stash the changes for later use
**Command**
```
$ git stash
```
> This command takes the uncommitted changes (both staged and unstaged), saves them away for later use, and then reverts them from your working copy.

## 20. Re-applying stashed changes
**Command**
```
$ git stash pop
```

## 21. Create Tags
**Command**
```
$ git tag <tagname>
```
**Example**
```
$ git tag 2022.05
```
## 22. List all Tags
**Command**
```
$ git tag -l
```
## 23. List the remote name
**Command**
```
$ git remote
```
## 24. List all the remotes
**Command**
```
$ git remote -v
```
## 25. List the commit logs
**Command**
```
$ git log
```
## 26. Print the commit logs
**Command**
```
$ git log -p
```
## 27. Reverting the commit
**Command**
```
$ git revert <commit>
```
**Example**
```
$ git revert d8ed902ffe7c1529d02d9a4857c1f541e2e0ce27
```
## 28. Replace the previous commit message
**Command**
```
$ git commit --amend -m "New commit message"
```
**Example**
```
$ git commit --amend -m "Updated message"
```
## 29. Searching in git
**Command**
```
$ git grep <searchable string>
```
**Example**
```
$ git grep "foo()"
```
## 30. Revert a git pull or move to a specific version of your code
**Command**
```
$ git reflog
$ git reset --hard <commit ID>
```
> `git reflog` will give the list of commit hashID's
> `git reset --hard <commit ID>` will only make changes in local repo
> `git push --force` is required if changes has to be pushed to remote server

**Example**
```
$ git reset --hard 95377807
```
> This will move our code into previous commit with ID 95377807