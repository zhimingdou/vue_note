# 
+ 安装git
+ git --version 查看版本
+ 
+ git config --global user.name "xiaodou" 配置
+ git config --global user.email "443903845@qq.com" 配置
+ git config --list  查看所有的已配置
+ git init  CD到一个目录里运行该命令 即可初始化项目（文件夹/目录,把这个目录变成一个仓库 或者git init 后面加目录名，就能初始化该目录（没有该目录会创建该目录）
+ ls -la 查看文件夹的文件 包括隐藏文件
+ git clone git地址  即可克隆一个项目到本地
+ git status 查看项目状态
+ git add . 把所有修改后的项目保存在暂存区（只保存在本地，并没有上传），每一次保存都是一次存档，可以回到之前的存档 ，如果后面的.写成文件名即只保存此文件
+ git commit -m "修改了xxx"  添加备注
+ git log 查看历史版本 按Q退出
+ git log -p 查看修改了什么内容 
+ git checkout xxx 查看历史的某一个版本 xxx是commit 的ID号 前七位即可
+ git checkout - 回到上一个版本，不管上一次操作的是哪个版本 
+ git tag -a v1 -m "第一个大版本"  用tag分割成大版本

### 创建分支
+ 主线是master 可以创建分支branch ，相当平行时空
+ git branch xxx(分支名)  创建分支
+ git checkout xxx    切换到分支
+ git log --oneline 查看状态
+ git checkout master 切换回到主线
+ git log --oneline --all --graph 图形化显示主线和分支 
+ git merge xxx（分支名） 合并分支 如果合并文件有冲突，可手动修改，因为是自己写的代码，所以知道手动怎么改

### 远程仓库
+ git remote add 自定义名 地址   //连接远程仓库
+ git remote -v  //查看当地连接的所有远程仓库
+ git push -u 自定义名 分支名（一般是主线master） //上传代码



从远程拉取代码到本地上
git clone 地址

#### 写完或者修改完代码
#### 添加到暂存区
+ git add . 
+ git commit -m "备注修改了什么"

#### 上传到远程仓库
+ git push -u origin master

#### 要是本地没有连接到远程仓库就
+ git remote add 名字（自定义，作为上传时 -u 后的名字）地址
+ git pull 更新本地项目 别的电脑或者别的人改变了本项目的远程仓库代码，这个命令可以把本地的代码，更新和远程仓库的代码一样
+ 
+ 
+ 
排除问题 遇到过的问题
进错文件夹，要是从远程仓库拉取的代码，git remote 一定有个origin,没有就是进错了


4.19
methods没加s
参数传错
