---
title: CREATE_BLOG
date: 2025-07-21 12:48:09
tags:
---

**创建一份个人博客**

------

创建博客文件夹

```
//目录名称不含空格的时候双引号可以省略
hexo init "你的博客目录名称"

/进入博客
cd "BLOG_"

//安装的依赖项在package.json文件的dependencies字段中可以看到
npm install 
```



写一篇新文章所需要的指令：

```
//会在 source/_posts/ 目录下生成文件 ‘test.md’，打开编辑
hexo new post "test" 

//生成静态HTML文件到 /public 文件夹中
hexo generate  

//本地运行server服务预览，打开 http://localhost:4000 即可预览你的博客
hexo server        
```



设置和更改主题

```
//git操作；拉取项目地址；标准存放文件夹
git clone https://github.com/litten/hexo-theme-yilia.git themes/yilia
```

将页面布置到github作为静态页面

```
//npm安装git插件，并且在自己的_config.yml进行更改
npm install hexo-deployer-git --save
```

_config.yml：

```
# Extensions
## Plugins: https://hexo.io/plugins/
## Themes: https://hexo.io/themes/
# 更改主题为开源主题yilia
theme: yilia

# Deployment
## Docs: https://hexo.io/docs/one-command-deployment
# 设置自己的推流网页
deploy:
  type: 'git'
  repo:  https://github.com/ANDyerGo/ANDyerGo.github.io.git
  branch: master
```























Git:免费开源的版本控制系统

