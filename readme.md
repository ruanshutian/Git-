### [git网址](https://git-scm.com/book/zh/v2/%E8%B5%B7%E6%AD%A5-%E5%AE%89%E8%A3%85-Git)

## 配置user信息

git config --global user.name "your_name"
git config --global user.email "your_email@domail.com"

git config --local :只对某个仓库有效
git config --global:对当前用户的所有仓库有效
git config --system:对系统所有登陆的用户有效



## 建git仓库
### 1 把已有的项目代码纳入git管理
cd 项目代码所在的文件夹
git init 

### 2 新建的项目直接用Git管理
cd 某个文件夹
git init your_project  # 会在当前路径下创建和项目名称同名的文件夹
cd your_project

git add .
or
git add xxx
git commit -m "reason"


### git 重命名
git mv readme.md readme
从readme.md变更命名到readme

### 查看版本历史
git log

### 查看分支
git branch

### .git文件夹里面
HEAD    显示在哪个分支
config  配置信息
refs    
objects

### 删除分支
 git branch -D xxx

### 修改最新commit的message信息
git commit --amend


## 上传本地仓库到远端
git remote add github git@github.com:ruanshutian/gitTest.git
git push github --all
git remote add xxx git@github.com:ruanshutian/gitTest.git
git push xxx --all




