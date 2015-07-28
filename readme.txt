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