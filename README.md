# Git Bash tricks

Ce HOU,

Mar 4, 2023

reference: [知乎：用git创建本地仓库并上传到Github](https://zhuanlan.zhihu.com/p/43225311)

## 1. 进入桌面创建一个目录并进入该目录
进入想要建立github repo的目录，并进入



## 2. 创建一个.git仓库

命令：`git init`:  在git-demo里创建一个.git仓库

`ls -a`: 查看git-demo里的所有文件，验证仓库是否创建成功

## 3. 将文件添加到暂存区

`git add css/style.css`: 添加**单个文件**（css/style.css）文件到暂存区

`git status -sb`: 获取文件的当前状态

`git add .`: 将当前**目录下所有变动文件**都加到暂存区

## 4. 将暂存区的文件添加到本地仓库

`git commit -m "xxx"`: 将代码添加至github repo上，并添加"xxx"的注释

## 5. 在GitHub上创建一个仓库，命名为git-demo

创建一个与本地仓库同名的线上仓库，并复制它下面的远程连接代码将本地与github链接

![远程代码演示](https://pic4.zhimg.com/v2-4737360fa603c5709b3d3ab131012083_r.jpg "远程代码演示")

## 6. 已有仓库，进行后续代码的更新

在更新前，先用`git pull`将线上仓库的代码更新到本地，确保两端信息同步

之后使用以下指令组合完成：
* `git add .`: 将所有更新添加至上传序列
* `git commit -m "type some annotation"`: 将代码传至push进程中
* `git push`: 将代码传至线上repo
