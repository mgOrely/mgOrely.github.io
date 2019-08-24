---
layout: post
title: "nginx location root alias"
description: "nginx location root alias"
keywords: "nginx, location, root, alias"
category: "nginx"
tags: [nginx,location,root,alias]
---

## 参考资料
[nginx的location、root、alias指令用法和区别](http://www.nginx.cn/4658.html)

## location+root/alias
root与alias主要区别在于nginx如何解释location后面的uri，这会使两者分别以不同的方式将请求映射到服务器文件上。
root的处理结果是：root路径＋location路径
alias的处理结果是：使用alias路径替换location路径
alias是一个目录别名的定义，root则是最上层目录的定义。
还有一个重要的区别是alias后面必须要用“/”结束，否则会找不到文件的。。。而root则可有可无~~

## location+proxy-pass


