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