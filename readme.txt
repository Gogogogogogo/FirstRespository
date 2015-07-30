Git is a version control system
Git is free

git init  //将一个目录变成一个git仓库 
git add <file> //将新增或者修改后的文件添加到仓库
git commit -m "提交说明" //提交

git status //查看仓库当前的状态
git diff   //查看

git log //查看历史记录
git reset --hard HEAD^ //版本的回退,回退到上一个版本
git reset --hard HEAD^^^ //回退到前三个版本
git reset --hard HEAD~100 //回退到前100个版本

//通过commit id来进行版本的更换
git reset --hard 37606199a3dc9198eb8cffd73763537a56298aaf
git reflog //查看所有的commit版本和commit id

使用git add 添加文件 实际上是把文件修改添加到暂存区；
使用git commit 提交 实际上就是把暂存区的所有内容提交到
当前分支

git追踪并管理的是修改而非文件，每次修改如果不add到暂存区，那就commit不到分支中

git checkout -- file :把工作区的修改全部撤销

一种是readme.txt自修改后还没有被放到暂存区，现在，撤销修改就回到和版本库一模一样的状态；

一种是readme.txt已经添加到暂存区后，又作了修改，现在，撤销修改就回到添加到暂存区后的状态。
git reset HEAD file可以把暂存区的修改撤销掉（unstage），重新放回工作区
git rm //用来删除版本库中的文件
git checkout -- <file> //git checkout其实是用版本库里的版本替换工作区的版本，无论工作区是修改还是删除，都可以“一键还原”

ssh-keygen -t rsa -C "youremail@example.com" //成功公钥和密钥对

git remote add origin 地址 //添加远程仓库地址
git push -u origin master //本地库的内容推送到远程，第一次推送 加上-u git不但会把本地master分支内容推送到远程新的master 分支，还会把本地的master分支和远程的master 分支关联起来