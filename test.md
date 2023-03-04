# Git Bash tricks

Ce HOU,

Mar 4, 2023

reference: [知乎：用git创建本地仓库并上传到Github](https://zhuanlan.zhihu.com/p/43225311)

# 1. 进入桌面创建一个目录并进入该目录
进入想要建立github repo的目录，并进入



# 2. 创建一个.git仓库

命令：`git init`:  在git-demo里创建一个.git仓库

`ls -a`: 查看git-demo里的所有文件，验证仓库是否创建成功

# 3. 将文件添加到暂存区

`git add css/style.css`: 添加**单个文件**（css/style.css）文件到暂存区

`git status -sb`: 获取文件的当前状态

`git add .`: 将当前**目录下所有变动文件**都加到暂存区

## 4. 将暂存区的文件添加到本地仓库

`git commit -m "xxx"`: 将代码添加至