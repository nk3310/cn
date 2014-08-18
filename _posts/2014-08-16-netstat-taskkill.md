---
layout: post
title: 联合使用netstat taskkill 终止jekyll server
categories: [technology]
tags: [jekyll server]
---

**起因:**

执行jekyll server提示4000端口己在使用。

**操作:**

 1, netstat -aon | findstr "4000" , 
     <pre>
     TCP    0.0.0.0:4000           0.0.0.0:0              LISTENING       6652
     </pre>
     
 2, tasklist | findstr "6652"
     <pre>
     ruby.exe                     6652 Console                    1     32,184 K
     </pre>
 
 3, taskkill /F /PID 6652
     <pre>
     成功: 已终止 PID 为 6652 的进程。
     </pre>
 
