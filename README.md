# mac安装环境时遇到的问题

### mac安装maven后重启terminal mvn指令not found. https://blog.csdn.net/With_Her/article/details/104144109


# Git
* git branch
* git branch -a
* git checkout -b branchname
* git push -u origin branchname
* git checkout branchname
* you are not allowed to push code to this project, git 权限不是developer是reporter


## Git rebase流程
* 1.git add. 2.git commit -m "commit message" 3.git rebase 4.git rebase -i HEAD~3(数字代表合几个commit）5.然后把第一个commit保留pick开头，把下面的commit开头改为s（后面加空格）6.git log看看刚才合并的commit是不是在一个 7.git push -f origin dev_userinfo (强行push）8.发现behind落后dev分支 9.git checkout dev/ git pull origin dev 10.git checkout dev_userinfo/ git pull from origin. 11.放弃rebase的话, git rebase --abort
* https://juejin.cn/post/6844903600976576519


# Terminal   
* Perminssion Denied 问题先试试+sudo

# Permission denined when building proejct
* dongziming@dongzimingdeMacBook-Pro aiworks % sudo chmod -R 777 *

# mvn clean package完文件全变蓝然后先跑通服务器再
* git stash 
* 记得clear stash！
