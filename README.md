## Git Commands Cheatsheet 
Steps to do 


```shell
https://git-scm.com/
```

Download git from official site
---

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
>> git fetch --dry-run
>> git fetch // remote to local
>> git merge //If we use fetch then call merge also to get changes in local files

#### PULL COMMAND
------------------
>> git pull
>> git pull origin master //pull from remote master branch 

>> git clone PROJECT_URL

>> git remote prune origin

>> git diff

#### Shortcut
git add . && git commit -m 'COMMIT MESSAGE' && git push origin BRANCH_NAME

