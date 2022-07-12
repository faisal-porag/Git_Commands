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

>> git status   //Get status summary

>> git add --all OR git add -A  //Both of means up all files on the stage
>> git add .                    //Means up all files on the stage in a specific folder
>> git add *                    //Up all files on the stage except deleted files
>> git add abc.txt              //Up specific files on the stage
>> git add *.js                 //Up same extension files on the stage

>> git reset    //Back from stage 

>> git commit -m "changes summary"

>> git reset HEAD~  //reset after commit apply
>> git reset --hard //deleted files also Back

>> git branch //get current branch
>> git branch development //Create new branch
>> git checkout development //Swtich to development branch

#### FOR DELETE LOCAL BRANCH 
>> git branch -d development
>> git branch -D development

>> git branch -b new_feature //Create and switch branch

>> git merge main -m "description u want" //Marge with main branch

#### IF UPLOAD FOR THE FIRST TIME THEN
--------------------------------------
>> git remote add origin (remote repository URL) like git remote add origin https://github.com/Faisal-CSE/Classic-ASP-Test
>> git remote -v

>> git push origin main         //push to remote in main branch
>> git push origin development  //push to remote in development branch

#### OPTIONAL
-------------
>> git push --set-upstream origin master //Push to remote 


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

