## Git Commands Cheatsheet 
Steps to do 


Download git from official site
---
```shell
https://git-scm.com/

---

#### set global git config settings

```sh 
git config --global --edit
```
---

```
#### COMMANDS (GIT INITIALIZE)

```shell
git init
```

#### Get status summary
```shell 
git status   
```
#### Both of means up all files on the stage
```shell
git add --all OR git add -A
```
#### Means up all files on the stage in a specific folder
```shell
git add .                    
```
#### Up all files on the stage except deleted files
```shell
git add *                    
```
#### Up specific files on the stage
```shell
git add abc.txt              
```

#### Up same extension files on the stage
```shell
git add *.js  
```
#### Back from stage 
```shell
git reset    
```
#### Commit
```shell
git commit -m "changes summary"
```
#### reset after commit apply
```shell
git reset HEAD~  
```
#### deleted files also Back
```shell
git reset --hard 
```
#### get current branch
```shell
git branch 
```
#### Create new branch
```shell
git branch development 
```
#### Swtich to development branch
```shell 
git checkout development 
```

#### FOR DELETE LOCAL BRANCH 
```shell 
git branch -d development
```
```shell
git branch -D development
```
#### Create and switch branch
```shell
git branch -b new_feature 
```
#### Marge with main branch
```shell 
git merge main -m "description u want" 
```

#### IF UPLOAD FOR THE FIRST TIME THEN
--------------------------------------
```shell
git remote add origin (remote repository URL) like git remote add origin https://github.com/Faisal-CSE/Classic-ASP-Test
```

```shell
git remote -v
```
####  push to remote in main branch
```shell
git push origin main    
```    
#### push to remote in development branch
```shell
git push origin development 
```

#### OPTIONAL (//Push to remote)
```shell
git push --set-upstream origin master  
```


#### FATCH COMMAND
------------------
```shell
git fetch --dry-run
```
#### remote to local
```shell
git fetch 
```
##### If we use fetch then call merge also to get changes in local files
```shell
git merge 
```

#### PULL COMMAND
------------------
```shell
git pull
```
#### pull from remote master branch 
```shell
git pull origin master
```

```shell
git clone PROJECT_URL
```

```shell
git remote prune origin
```

```shell
git diff
```

#### Shortcut
```shell
git add . && git commit -m 'COMMIT MESSAGE' && git push origin BRANCH_NAME
```

```shell
git log
```
#### clean remote branch in locally 
```shell 
git remote prune origin
```

#### Publish your tags
```shell
git push --tags
```

#### Revert a commit (by producing a new commit with contrary changes)
```shell
git revert <commit>
```
#### Discard all local changes in your working directory
```shell
git reset --hard HEAD
```

#### Reset your HEAD pointer to a previous commit & preserve uncommitted local changes
```shell
git reset --keep <commit>
```

#### Delete a branch on the remote
```shell
git branch -dr <remote/branch>
```
---

#### Force commit to the remote branch (Revert process)
```shell
git push origin <commit SHA>:<remotebranchname> -f
```
Example: `git push origin YOUR_COMMIT_ID:REMOTE_BRANCH_NAME -f`

---

#### reset local branch 
```shell
git reset YOUR_COMMIT_ID
```


#### GIT DETAILS LOG BY COMMIT ID 
```shell
git diff-tree --no-commit-id --name-only -r 61043e098f9b8526f6c1abd910d40e5fd7d7deae
or ------- 
git log --name-only
```


##### SHOW COMMIT DETAILS LOG
```sh 
git show <COMMIT_ID>
```

unstage a file while retaining the changes in working directory
```sh
git reset <FILE_NAME>
```

---

##### TEMPORARY COMMITS

Save modified and staged changes
```sh
git stash
```

list stack-order of stashed file changes
```sh 
git stash list
```

write working from top of stash stack
```sh
git stash pop
```

discard the changes from top of stash stack
```sh
git stash drop
```
---






