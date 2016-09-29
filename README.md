# xdevcp.github.com
https://github.com/xdevcp/xdevcp.github.com.git

http://x.devcp.org

## HEXO
https://hexo.io/
```
npm install hexo-cli -g
hexo init blog
cd blog
npm install
hexo server
```

原文链接：http://www.jianshu.com/p/701b1095da11

## hexo使用
目录结构
```
.
├── .deploy #需要部署的文件
├── node_modules #Hexo插件
├── public #生成的静态网页文件
├── scaffolds #模板
├── source #博客正文和其他源文件，404、favicon、CNAME 都应该放在这里
| ├── _drafts #草稿
| └── _posts #文章
├── themes #主题
├── _config.yml #全局配置文件
└── package.json
```

## hexo命令行使用

常用命令：
```
hexo help #查看帮助
hexo init #初始化一个目录
hexo new "postName" #新建文章
hexo new page "pageName" #新建页面
hexo generate #生成网页，可以在 public 目录查看整个网站的文件
hexo server #本地预览，'Ctrl+C'关闭
hexo deploy #部署.deploy目录
hexo clean #清除缓存，**强烈建议每次执行命令前先清理缓存，每次部署前先删除 .deploy 文件夹**
```
简写：
```
hexo n == hexo new
hexo g == hexo generate
hexo s == hexo server
hexo d == hexo deploy
```

## 编辑文章

新建文章

hexo new "标题"

在 _posts 目录下会生成文件标题.md
```
title: Hello World
date: 2015-07-30 07:56:29 #发表日期，一般不改动
categories: hexo #文章文类
tags: [hexo,github] #文章标签，多于一项时用这种格式
```
---
正文，使用Markdown语法书写

编辑完后保存，hexo server 预览

## hexo部署

执行下列指令即可完成部署。
```
hexo generate
hexo deploy
```
以下提示说明部署成功
`
[info] Deploy done: git
`



