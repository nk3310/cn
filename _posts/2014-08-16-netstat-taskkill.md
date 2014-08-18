---
layout: post
title: 联合使用netstat taskkill 终止jekyll server
categories: [technology]
tags: [jekyll server]
---

起因:

执行jekyll server提示4000端口己在使用。

操作:

 1. netstat -aon | findstr "4000" , 
 
   列出PID号如下：
 
   TCP    0.0.0.0:4000           0.0.0.0:0              LISTENING       6652

 2. taskkill /F /PID 6652
 
