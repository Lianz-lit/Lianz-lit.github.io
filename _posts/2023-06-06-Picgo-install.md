---
layout:       post
title:        "安装Picgo"
author:       "Lianz"
header-style: text
catalog:      true
tags:
    - install
    - Mac
---

> 安装Picgo时，提示已损坏，无法打开，请移至废纸篓

目录

[toc]

# 安装环境

m1 pro，ventura 13.1

# 安装包

PicGo-2.3.1-arm64.dmg

下载链接：https://github.com/Molunerfinn/PicGo/releases/tag/v2.3.1

# 解决方案

第一步，因为Mac在安装来自第三方的软件时，会进行验证。在`System Settings/Privacy&Security`路径下的Security中，应当显示`Anywhere（任何来源）`的选项。如果该选项被隐藏，可以通过在terminal中输入下面语句显示该选项。

`sudo spctl  --master-disable`

输入命令后回车，会被要求输入开机密码，输入完成后回车即可。再次打开打开Security可以看到选项正常显示：

![](https://cdn.jsdelivr.net/gh/Lianz-lit/notes-pic/202306131958002.png)



第二步，在terminal中输入下面的语句并回车，输入开机密码回车。其中，`com.apple.quarantine`以及空格后面的内容为软件的路径，将软件拖入terminal可以快速获得该软件路径。

`sudo xattr -r -d com.apple.quarantine /Applications/PicGo.app`

