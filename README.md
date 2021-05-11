# git
Git（读音为/gɪt/）是一个开源的分布式版本控制系统，可以有效、高速地处理从很小到非常大的项目版本管理。 [1]  也是Linus Torvalds为了帮助管理Linux内核开发而开发的一个开放源码的版本控制软件。

目前市面使用的版本管理软件 主要分为两类
1. 集中式代码管理(svn)  5%
2. 分布式代码管理(git)  95%

项目(源代码)管理软件 主要管理开发环境下的软件的源码(自己写的代码)

官网:
https://git-scm.com/
git是一个跨平台的版本管理工具(windows linux unix osx)

### git基本操作

### 用户设置
```bash
### 全局用户设置 每台新的电脑仅需一次设置
$ git config --global user.name 'Zhang Jun'
$ git config --gulbal user.email 'root@rootbk.cn'
```

1. 项目构建 项目目录(README.md .gitignore)
2. 在项目根目录下初始化本地仓库 `$ git init`
3. 初始化node项目 `$ npm init -y`

### 常用指令
```bash
# 查看状态
$ git status

# 添加管理(将文件添加到本地仓库的暂存区)
$ git add fileName      # 将指定文件添加到git仓库的暂存区
$ git add .             # 将当前目录下所有文件和目录都添加到git仓库的暂存区
$ git add --all         # 将当前目录下所有文件和目录都添加到git仓库的暂存区
$ git add path/         # 将指定目录添加到暂存区

# 将文件移出暂存区
$ git rm --cached fileName

# 将暂存区的文件提交到本地仓库
$ git commit -m 'msg'
```