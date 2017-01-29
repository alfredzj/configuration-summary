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

##
