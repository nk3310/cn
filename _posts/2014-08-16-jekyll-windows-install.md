---
layout: post
title: jekyll install 回顾
categories: [technology]
tags: [jekyll install]
---

github.io上的第二篇BLOG: jekyll windows install 回顾。

1: http://jekyllcn.com/docs/installation/ 下载ruby和DevKit。

2: http://www.madhur.co.in/blog/2011/09/01/runningjekyllwindows.html 4步骤后执行一遍 gem update --system

3: http://www.madhur.co.in/blog/2011/09/01/runningjekyllwindows.html 7,8,9步骤安装Python不必做。

4：默认的 jekyll new myblog生成的_posts/*-welcome-to-jekyll.markdown 含有语法加亮highlight ruby，需要执行gem install rouge， _config.yml中加入highlighter: rouge。
   [参见这里](http://stackoverflow.com/questions/16498287/jekyll-liquid-exception-cannot-load-such-file-yajl-2-0-yajl)。

