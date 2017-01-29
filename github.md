# Git & Github

## How to connect your PC to Github
> git config --global user.name "My Name"   
> git config --global user.email myEmail@example.com 

## How to initialize a repository
> cd /some_address/     
> git init

## How to look for the status of the files
> git status

## Add the file to the index (Aka the cache or staging area)
> git add     
> git rm

## Commit the file
> git commit -m "Initial commit"


-------------------------------------------------------------------------
##### The above operations are done locally
------------------------------------------------------------------------- 

## Link the remote repository
> git remote add origin git@github.com:alfredzj/Study-Note.git

## Push your files to github
> git push origin master    
(There are two parameters. The first one is the name of repository and the second is the name of branch.)

## Download the code to the PC
> git clone git@github.com:alfredzj/Study-Note.git    
> git pull origin master

## Branch
![Image of Branch](https://github.com/alfredzj/Study-Note/blob/master/pics/branch_git)          
It is good to use branch because    
* The stable version will not be destroyed
* Good for developers in a team

### Create a Branch
> git branch this_is_a_branch

### Look for and change the branches
> git branch
> git checkout this_is_a_branch

### How to merge branches
e.g: we first create a file on this_is_a_branch and then merge it with master
> git add abc.txt               
> git commit -m "this is done on this_is_a_branch"              
> git checkout master           
> git merge this_is_a_branch            
> git branch -d this_is_a_branch                







        
[Reference](https://mp.weixin.qq.com/s?__biz=MzAxODI5ODMwOA==&mid=2666539259&idx=1&sn=b139740a5d2c1fea22d2f1087eb01761&scene=2&srcid=06298zkT5e0P6jWl9VVE9inj&from=timeline&isappinstalled=0#wechat_redirect)
 
