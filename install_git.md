# 安装git
* ubuntu Linux
```java
$ git
The program 'git' is currently not installed. You can install it by typing:
```
表示本机还没有添加git
### 使用下面的命令进行安装git工具.
```java
sudo apt-get install git
```
# 创建git版本库
### 1. 第一步, 先要创建一个目录, 这个目录就是用来存放仓库的.
```java
$ mkdir html
$ cd html
```
### 2. 第二步, 使用git init命令, 将当前目录创建成git仓库.
创建文件 并进行提交 设置默认编辑器为 vim
```touch README
im README
git status
git add README
git commit 
git config --global user.name  "自己的姓名"
git config --global user.email “自己邮件”
git config --global core.editor vim
git commit 
```
然后可以查看自己信息
```
git log
git status
```
### 第三步 添加远程仓库
```
git remote add origin https://github.com/wangleihd/h5class.git
```
### 第四部 向远程仓库提交
```
$ git push origin master
$ git push origin branch-name
```
### 第五步 从远程仓库更新到本地
```
git pull origin master
```
