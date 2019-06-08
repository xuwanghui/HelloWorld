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
- `git branch "分支名字"`

- 合并时如果有冲突,需要手动处理,处理后需要再提交一次

## GitHub
- 不是git,只是一个网站
- 只不过这个网站提供了允许别人通过git上传代码的功能

### 提交代码到GitHub(当作git服务器来用)
- `git push [地址] master`
    + 示例: git push https://github.com/xuwanghui/HelloWorld.git master

    + 会把当前分支的内容上传到远程的master分支上

- `git pull [地址] master`
    + 示例: `git pull https://github.com/xuwanghui/HelloWorld.git master`
    + 会把远程分支的数据得到:(*注意:本地要初始化一个仓储*);

- `git clone [地址]`
    + 会得到远程仓储相同的数据,如果多次执行会覆盖本地的内容

## SSH 方式上传代码
- 不需要输入账号和密码就可以验证上传者的身份
- 公钥 私钥,两者之间是有关联的
- 生成公钥和私钥
    + `ssh-keygen -t rsa -C "邮箱"`