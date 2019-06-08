## git 安装

## 初始化git仓库
- 这个仓库会存放,git对我们项目代码进行备份的文件
- 在项目目录右键打开 git bash
- 命令： `git init`

## 自报家门
- 就是在git设置当前使用的用户是谁(避免提交代码冲突)
- 每一次备份都会把当前备份者的信息存储起来
- 命令：
    + 配置用户名：`git config --global user.name "用户名"`
    + 配置邮箱：`git config --global email "邮箱"`

## 把代码存储到.git仓储中
- 1. 把代码放到仓储的门口
    + `git add ./READEME.md`
    + `git add ./` 
- 2. 把仓储门口的代码放到里面的房间
    + `git commit -m "对这次添加的代码的解释说明"`
    + `git commit `
## 把大象放进冰箱需要几步

## 查看当前git状态
- 可以查看当前代码是否被放到了仓储中
- 命令：`git status`

## 如何直接把代码放到仓储而不放到大门口

## 回退到指定版本
- `git reset --hard Hearder~0`

## git创建分支,切换分支