# 开源硬件模块芯片

> 原文：<https://hackaday.com/2013/09/17/an-open-source-hardware-modchip/>

[![OSHW XenoGC Clone](img/b21549121041eaf02c2243929226e0fc.png)](http://hackaday.com/?attachment_id=103171)

许多 Hackaday 读者可能还记得从有些可疑的来源购买 modchips 的日子。这些小设备连接到一个游戏系统来绕过安全措施，允许你运行自制游戏(和盗版游戏，但我们不关注这一点)。Guillermo 基于 XenoGC 构建了一个开源硬件 Gamecube modchip。

XenoGC 在 Gamecube 时代是一种流行的 modchip，它的来源在一个论坛帖子中发布。一个[维基页面](http://www.gc-forever.com/wiki/index.php?title=XenoGC_Clone "XenoGC Clone on GC Forever")解释了如何基于 ATtiny2313 构建该设备的克隆版。大多数 modchips 都是闭源的，但是这个项目可以让你看到它们是如何工作的。你可以在[的谷歌代码](https://code.google.com/p/xenogcfork/source/browse/#svn%2Ftrunk) "XenoGC on Google Code")上浏览 XenoGC 源代码，了解更多关于漏洞本身的信息。你可以在 XenoAT 文件夹中找到 AVR 代码，它通过串行接口操纵 DVD 驱动器。

[Guillermo]的硬件可从 [OSHPark](//oshpark.com/shared_projects/FV4wrWMl) 获得，因此您可以轻松订购电路板。他还在 [Github](https://github.com/gamaral/XenoGC "XenoGC") 上托管设计文件。有了一个在手，你就可以开始为 Gamecube 自制程序了，现在花 25 美元左右就能买到。