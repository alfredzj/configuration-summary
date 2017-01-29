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



------------------------------------------------------

查看当前状态 $ git status 
查看远程仓库：$ git remote -v  
查看分支 $ git branch  
查看历史日志 $  git log

$ git  clone  git://github.com/someone/some_project.git  some_project  #将'git://github.com/someone/some_project.git'这个URL地址的远程版本库，完全克隆到本地some_project目录下
git clone -b <branch> <remote_repo>   #只克隆某个分支
添加远程仓库：$ git remote add [name] [url]
git  remote  add  origin  git://github.com/someone/another_project.git #增加URL地址为'git: //github.com/someone/another_project.git'，名称为origin的远程服务器，以后提交代码的时候只需要使用 origin别名即可


删除远程仓库：$ git remote rm [name]
修改远程仓库：$ git remote set-url --push [name] [newUrl]
拉取远程仓库：$ git pull [remoteName] [localBranchName]
推送远程仓库：$ git push [remoteName] [localBranchName]


查看当前分支：$ git branch -a
创建本地分支：$ git branch [name] ----注意新分支创建后不会自动切换为当前分支
切换分支：$ git checkout [name]
创建新分支并立即切换到新分支：$ git checkout -b [name]
创建本地分支,并指定远程分支的对应关系: $ git checkout -b gitcafe-pages remotes/origin/gitcafe-pages
删除分支：$ git branch -d [name] ---- -d选项只能删除已经参与了合并的分支，对于未有合并的分支是无法删除的。如果想强制删除一个分支，可以使用-D选项
合并分支：$ git merge [name] ----将名称为[name]的分支与当前分支合并


git revert：还原一个版本的修改，必须提供一个具体的Git版本号，例如'git revert bbaf6fb5060b4875b18ff9ff637ce118256d6f20'，Git的版本号都是生成的一个哈希值


        
[Reference](https://mp.weixin.qq.com/s?__biz=MzAxODI5ODMwOA==&mid=2666539259&idx=1&sn=b139740a5d2c1fea22d2f1087eb01761&scene=2&srcid=06298zkT5e0P6jWl9VVE9inj&from=timeline&isappinstalled=0#wechat_redirect)
 
