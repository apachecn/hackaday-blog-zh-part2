# 黑客日复古版:TRS 维基

> 原文：<https://hackaday.com/2015/04/28/hackaday-retro-edition-trs-wiki/>

1977 年对于计算历史来说是特殊的一年；继一年前发布 Z80 之后，今年又发布了 8085。三家公司将在 1977 年推出他们的第一台真正的生产计算机:苹果发布了 Apple II，Commodore the PET 2001，Tandy / Radio Shack 的 TRS-80 Model I。这些都是令人难以置信的有限的机器，但至少其中一台[仍然可以用来浏览维基百科](http://pski.net/trswiki/)。

[Pete]的 TRSWiki 是 TRS-80 模型 I 的维基百科客户端，它能够查找数百万篇只有大写字符和低分辨率(128×48)图形的文章。它通过一个非常酷的 [Model I 系统扩展器](http://home.comcast.net/~bartlett.p/MISE/) (MISE)通过以太网实现这一点，将低级的 Trash-80 带入现代时代。

MISE 能够从 CF 卡启动，驱动 SVGA 显示器并连接到 10/100 以太网。通过以太网连接互联网是一回事，但请求和加载网页完全是另一回事。TRS-80 的内存不太可能容纳大图像或巨大的文本墙，所以[皮特]在亚马逊网络服务盒子上使用代理服务器。这个代理是用 Java 写的，但是在 TRS-80 上运行的代码完全是用 Z80 汇编写的；对于[Pete]在 Z80 装配中的第一个项目来说还不错。

* * *

![vt100normal](img/feb3dafab4e4c1a5d2af53414a3bdeb2.png)hack aday 复古版是我们庆祝旧电脑做一些现代的事情，在大多数情况下，加载旧的，没有 CSS 或 Javascript 版本的我们的网站。

如果你有一台想要展示的旧电脑，只需加载复古网站，抓拍一些照片，将它们冲洗出来，[并发送到](http://hackaday.com/submit-a-tip/)。