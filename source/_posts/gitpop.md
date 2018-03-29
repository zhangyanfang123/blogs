---
title: 用命令行将项目传到github
tags: git
categories: 工具
---
### 步骤如下
#### 1.安装git后，打开cmd，进入要上传的文件夹中；
#### 2.输入`git init` 初始化本地git仓库；
#### 3.`git add .``将所有文件提交到暂存区；
#### 4.`git commit -m'说明文字'`；
#### 5.`git remote add origin http://github...`(要关联的github地址)，关联github；
#### 6.`git pull origin master` ,将GitHub上的代码传到本地；
#### 7.`git push -u origin master`,第一次上传代码，如果没有意外就上传成功。
 ### 可能会有的报错：
#### 1.不算报错，它会提醒让你提交个人信息，输入：` git config user.email "123@gmail.com" git config user.name "rongy" `
#### 2.在 `git add .`后会显示on branch master nothing to commit,working directory clean,这说明你的文件已经commit过了，所以在add .就没用了,所以不用管它;
#### 3.在`git pull origin master`后，出现fatal: refusing to merge unrelated histories，出现这个应该是之前在github上用导入的方式导入过文件，我们再提交，本地的和github上的就没有共同祖先（原因是这个，但为什么我也不懂。。。），
就无法提交了，解决方法是输入`git pull origin master` --allow-unrelated-histories。
#### 4.并且在pull操作后的push操作，在命令后再加上备注名，即`git push -u origin master：master`
