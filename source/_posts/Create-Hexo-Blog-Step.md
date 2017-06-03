---
title: Create Hexo Blog Step
date: 2017-06-02 00:01:45
tags:
---

# 搭建步骤：
1.安装Git
2.安装Node.js
3.安装hexo：sudo npm install -g hexo
4.hexo init
5.hexo generate(hexo g)
6.hexo server(hexo s)-->本地localhost:4000查看是否搭建本地Blog成功
7.关联git
8.修改_config.yml
9.删除themes/landscape下第74-77行（提示主题出错）
10.npm install hexo-deployer-git --save
11.hexo deploy(hexo d)

# 使用命令：
1.hexo new "new post name"
2.hexo new page "new page name"
3.hexo clean
4.hexo generate(hexo g)
5.hexo deploy(hexo g)
6.hexo help
7.hexo version
8.通过git clone主题到themes下(git clone xxx.git themes/xxx)，修改_config.yml中的theme标签，更换主题

# 使用其他PC更新Blog：
1.通过分支方式，将原Blog文件夹下的文件提交到远程仓库另一分支：hexo
2..gitignore文件内容如下
 .DS_Store
 Thumbs.db
 .deploy_git/
 /node_modules/
 /public/
3.在其他PC将分支hexo上的文件pull下来
4.执行以下指令：
 npm install hexo
 npm install
 npm install hexo-deployer-git –save