---
title: virtualbox备份微信
date: 2017-07-21 19:03:37
tags:
    - virtualbox
    - win10
    - usb2.0
    - 微信备份
categories: 修理电脑
---
刚开始安装virtualbox没法用usb2.0,需要安装增强软件
- 查版本号：dpkg -l，找virtualbox对应的版本号
- 安装增强插件，网址https://www.virtualbox.org/wiki/Downloads
- 安装后把当前用户加到vboxuser用户组
- 查看所有用户组，cat /etc/group
- 加用户组，sudo usermod -G vboxusers -a
    ray，其中ray是你要使用vbox的当前用户名。重启以后就可以了
- 连了usb以后，需要把网络改成桥接模式，就可以用微信备份聊天记录了。。

记录一下过程，ubuntu下有个虚拟机还是方便很多的
