---
layout: post
title: ����ʹ��netstat taskkill ��ֹjekyll server
categories: [technology]
tags: [jekyll server]
---

##����
ִ��jekyll server��ʾ4000�˿ڼ���ʹ�á�

##����
* netstat -aon | findstr "4000" ,�г�PID�����£�
 TCP    0.0.0.0:4000           0.0.0.0:0              LISTENING       6652
* taskkill /F /PID 6652
 