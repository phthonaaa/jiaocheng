# Git使用

## 拉项目和上传项目

拉：$ git clone +链接（https://gitee.com/lo_cy/cppcheck.git）

上传：

## 1.git简介

1.1Git源代码管理工具，linus写的一个代码的版本管理工具。（备份管理）

版本控制工具有：svn、vss、vcs...git

1.2直接一直下一部安装

1.3初始化git仓储

在相应的存储的位置上目录下右击建立git bash

命令：‘git init’

![image-20210215112951079](C:\Users\Administrator\AppData\Roaming\Typora\typora-user-images\image-20210215112951079.png)

1.4在git中配置以下创作者的信息

即在git中设置当前的用户是谁

每次备份代码都会把备份者信息备份在其中去。

命令： 

配置用户名：git config --global user.name "QiCheng"

配置邮箱：	git config --global user.email "17308435883@163.com"

## 2.备份代码

### 2.1把代码存储到.git中

![image-20210215115538381](C:\Users\Administrator\AppData\Roaming\Typora\typora-user-images\image-20210215115538381.png)

![image-20210215115644028](C:\Users\Administrator\AppData\Roaming\Typora\typora-user-images\image-20210215115644028.png)

### 2.2在代码中有修改

比如：添加了功能

![image-20210215120749351](C:\Users\Administrator\AppData\Roaming\Typora\typora-user-images\image-20210215120749351.png)

### 2.3查看当前代码的状态

git status可以查看当前的代码的状态。

### 2.4直接添加到仓储中

git commit --all -m “说明”

![image-20210215133141932](C:\Users\Administrator\AppData\Roaming\Typora\typora-user-images\image-20210215133141932.png)

![image-20210215133206511](C:\Users\Administrator\AppData\Roaming\Typora\typora-user-images\image-20210215133206511.png)

## 3.查看提交的记录

![image-20210215133450452](C:\Users\Administrator\AppData\Roaming\Typora\typora-user-images\image-20210215133450452.png)

### 3.1查看日志

-‘git log ’查看历史提交的日志

-‘git log --oneline ’查看简洁版的日志

### 3.2代码的回退

git reset --hard Head~0

### 3.3通过版本号切换版本

git reset --hard [版本号]（可以删除已有的也可以找到被删除的）

第一次关掉命令窗口之后就可以使用命令：

git reflog     得到之前的版本号

![image-20210215135449438](C:\Users\Administrator\AppData\Roaming\Typora\typora-user-images\image-20210215135449438.png)

## 4.分支

### 4.1切换分支

![image-20210215150256529](C:\Users\Administrator\AppData\Roaming\Typora\typora-user-images\image-20210215150256529.png)

创建分支：git branch dev

![image-20210215151317368](C:\Users\Administrator\AppData\Roaming\Typora\typora-user-images\image-20210215151317368.png)

![image-20210215151332474](C:\Users\Administrator\AppData\Roaming\Typora\typora-user-images\image-20210215151332474.png)

### 4.2版本号和分支

![image-20210215151404404](C:\Users\Administrator\AppData\Roaming\Typora\typora-user-images\image-20210215151404404.png)

![image-20210224172133170](C:\Users\Administrator\AppData\Roaming\Typora\typora-user-images\image-20210224172133170.png)

### 4.3合并分支

![image-20210224173755627](C:\Users\Administrator\AppData\Roaming\Typora\typora-user-images\image-20210224173755627.png)

合并时出现冲突就需要我们手动去合并。

以上的方式是把我们的代码存储到本地的文件夹中，而且是以二进制的形式存储的，是个人的，用处很小。

![image-20210224174333558](C:\Users\Administrator\AppData\Roaming\Typora\typora-user-images\image-20210224174333558.png)

# 5.开发中使用git（这里用github）

### 5.1提交代码到github（当作git服务器）

