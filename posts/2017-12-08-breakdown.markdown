---
layout: post
title:  "APP模块划分"
categories: jekyll update
---

# App Repository Server

App仓库以及App所依赖的组件的仓库（部分npm包的镜像）。

# Single Sign On Server

用OAuth来达到SSO的效果，免除用户需要在各App中重新注册账号的烦恼。

存储多种用户资料，不光是用户基本信息，还可以是用户的车牌号、会员卡等。

真正上线后可以做 “资料权限”，每个App向服务运维商提交申请，审核通过后给这个App开所有用户的某些资料读取权限。

# App Discovery Server

App发现服务器，根据用户的GPS信息，返回App Repository Server的一些entry，

即告诉用户，在附近有哪些可以使用的App。

# On-premise  Server

## App Repository Cache / CDN

```App Repository Server```的CDN，根据用户的设置可缓存指定范围的App/库，以达到就近分发的效果。

## Local App Index Server

本地APP索引，接入某个WiFi后，发现额外的App。

即能返回给用户一系列App Repository Cache的入口。

# Android Client  + 桌面小工具 

安卓客户端可以主要以桌面小工具的方式存在。

拖动一个4*1的小工具到桌面上，就可以容纳下4个主动发现的App的图标。

如果发现的App数量多于4个，则可以左右拖动桌面小工具来显示下更多的。

安卓App打开，则主要是设置相关界面。

也可以加上附近的App、历史App、收藏的App等信息。
