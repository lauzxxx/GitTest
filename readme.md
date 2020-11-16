## readme 文档
1. readme文档可以是txt文件，也可以是md文档
2. 一般和项目放在一起，作为项目的说明文档


# 全局配置
1. 配置用户名 
2. 配置邮箱 
3. 一台电脑只需配置一次
4. 查看配置信息 git config --list

# GIT 使用
1. 在电脑上创建一个文件夹为工作区
2. 打开文件右键 git bash here 进入当前目录
3. 工作区持有项目实际文件


# 初始化
1. git init 初始化版本库
2. 当前目录路径后面有(master)代表初始化成功
3. 当前目录下会生成一个隐藏文件 .git 代表这是一个版本库
4. 千万别操作 .git文件，让他隐藏不管他


## 工作区内容提交到本地仓库
1. git add文件名，将工作区的内容提交到暂存区
2. 命令 git add . 将所有变动提交到暂存区
3. 从暂存区提交到本地仓库 git commit -m '提交注释'


## 版本回退
1. 命令：git reset --hard HEAD^ 回退到上一个版本（一个^代表上一个版本）
2. 命令：git rest --hard 版本号 回退到指定版本


## 辅助命令
1. 命令 git status 查看当前目录下的操作状态
2. git log 查看日志
3. git reflog 查看简版日志 


## 将本地仓库提交到远程仓库
1. 在gitHbu创建一个远程仓库 GitTest
2. 在本地工作区先提交到本地仓库
3. git remote add origin https://github.com/lauzxxx/GitTest.git 本地仓库和远程仓库关联
4. git remote -v 查看本地仓库所关联的远程仓库地址
5. git push -u origin master
git push 把本地仓库推送到远程仓库
-u origin master 设置默认提交master分支到origin


## 下载项目到本地
1. 克隆项目：git clone 项目远程仓库地址 整个版本库克隆下来
2. git clone 适用于本地没有该项目 直接从远程下载到本地
3. 如果本地有该项目，应该直接更新到本地 git pull
4. 一定要先把工作区的修改提交到本地仓库再更新远程到本地