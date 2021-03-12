## How to use Git?

### Introduction

* Git an open source, distributed version-control system.

* Key concepts

  - Working Directory: 在电脑里能看到的目录
  - Repository: 工作区有一个隐藏目录.git
  - Stage: Git的版本库里存了很多东西，其中最重要的就是称为stage（或者叫index）的暂存区，还有Git为我们自动创建的第一个分支master
  
> 第一步是用git add把文件添加进去，实际上就是把文件修改添加到暂存区；
  第二步是用git commit提交更改，实际上就是把暂存区的所有内容提交到当前分支。

#### set up: configuring user information used across all local repositories
- git config --global user.name “[firstname lastname]” \
  `set a name that is identifiable for credit when review version history`
- git config --global user.email “[valid-email]” \
  `set an email address that will be associated with each history marker`
- git config --global color.ui auto \
  `set automatic command line coloring for Git for easy reviewing`

#### set up & init: configuring user information, initializing and cloning repositories
- git init \
  `initialize an existing directory as a Git repository`
- git clone [url] \
  `retrieve an entire repository from a hosted location via URL`
  
#### stage & snapshot: working with snapshots and the Git staging area
- git status \
  `show modified files in working directory, staged for your next commit`
- git add [file] \
  `add a file as it looks now to your next commit (stage)`
- git reset [file] \
  `unstage a file while retaining the changes in working directory`
- git diff \
  `diff of what is changed but not staged  -> 暂存区和工作区`
- git diff --staged \
  `diff of what is staged but not yet commited -> 暂存区和上一次的commit`
- git commit -m “[descriptive message]” \
  `commit your staged content as a new commit snapshot`
  
#### branch & merge: isolating work in branches, changing context, and integrating changes
- git branch \
  `list your branches. a * will appear next to the currently active branch`
  `-a: print out the list; -d: delete specific local branch`
- git push origin --delete [branch-name] \
  `delete branch remotely; cannot delete default branch`
- git branch [branch-name] \
  `create a new branch at the current commit`
- git checkout [branch-name] \
  `switch to another branch and check it out into your working directory`
- git merge [branch] \
  `merge the specified branch’s history into the current one`
- git log \
  `show all commits in the current branch’s history`
  
#### inspect & compare: examining logs, diffs and object information
- git log \
  `show the commit history for the currently active branch`
- git log branchB..branchA \
  `show the commits on branchA that are not on branchB`
- git log --follow [file] \
  `show the commits that changed file, even across renames`
- git diff branchB...branchA \
  `show the diff of what is in branchA that is not in branchB`
- git show [SHA] \
  `show any object in Git in human-readable format`

#### tracking path changes: versioning file removes and path changes
- git rm [file] \
  `delete the file from project and stage the removal for commit`
- git mv [existing-path] [new-path] \
  `change an existing file path and stage the move`
  
#### share & update: retrieving updates from another repository and updating local repos
- git remote add [alias] [url] \
  `add a git URL as an alias`
- git fetch [alias] \
  `fetch down all the branches from that Git remote` 
- git merge [alias]/[branch] \
  `merge a remote branch into your current branch to bring it up to date` 
- git push [alias] [branch] \
  `Transmit local branch commits to the remote repository branch`   
- git pull \
  `fetch and merge any commits from the tracking remote branch`  
  
#### rewrite history: rewriting branches, updating commits and clearing history
- git rebase [branch] \
  `apply any commits of current branch ahead of specified one`
- git reset --hard [commit] \
  `clear staging area, rewrite working tree from specified commit`
