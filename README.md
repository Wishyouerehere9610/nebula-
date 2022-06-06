
# mac安装maven后重启terminal mvn指令not found. https://blog.csdn.net/With_Her/article/details/104144109

# Git
* git branch
* git branch -a
* git checkout -b branchname
* git push -u origin branchname
* git checkout branchname
* you are not allowed to push code to this project, git 权限不是developer是reporter
* git reset --hard HEAD^ 返回git的上一个版本

## SSL certificate problem: certificate has expired 
* git config --global user.name [username]
* git config --global user.email [email]
* git config --global http.sslVerify false
* 可以正常pull了

## Git rebase流程
* 1.git add. 2.git commit -m "commit message" 3.git rebase 4.git rebase -i HEAD~3(数字代表合几个commit）5.然后把第一个commit保留pick开头，把下面的commit开头改为s（后面加空格）6.git log看看刚才合并的commit是不是在一个 7.git push -f origin dev_userinfo (强行push）8.发现behind落后dev分支 9.git checkout dev/ git pull origin dev 10.git checkout dev_userinfo/ git pull from origin. 11.放弃rebase的话, git rebase --abort
* https://juejin.cn/post/6844903600976576519


# IntelliJ IDEA Springboot问题

* mvn clean package完文件全变蓝然后先跑通服务器再stash(试试先进root再mvn clean package)
* 用户进root: sudo su -
* root切换到用户: sudo su - dongziming 
* git stash 
* 记得 git stash clear

## debug mode
* step over 进行下一行
* step into 进入这一行的方法
* resume program 进入下一个断点

## Permission denined when building proejct
* dongziming@dongzimingdeMacBook-Pro aiworks % sudo chmod -R 777 *

## 解决循环依赖的方法
* 在service上面加@Lazy注释


# 服务器问题
## kill进程
* kill falsk 进程
* ps aux|grep flask 
* kill -9 进程号

* kill java 进程
** jps + kill -9 进程号

## uwsgi flask
* sh start.sh / sh stop.sh
* 看uwsgi_log tail -f uwsgi.log 



