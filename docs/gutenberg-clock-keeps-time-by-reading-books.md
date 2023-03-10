# 古腾堡钟通过看书来保持时间

> 原文：<https://hackaday.com/2014/08/13/gutenberg-clock-keeps-time-by-reading-books/>

[![Gutenberg clock displaying text from a book](img/b03d8b5e7e57fba0d6c56d027e0f4102.png)](http://hackaday.com/2014/08/13/gutenberg-clock-keeps-time-by-reading-books/screen-shot-2014-08-12-at-11-40-33-am/)

我们已经看到了各种各样保持时间的黑客，但[ch00f]的最新版本在计算秒方面有了新的突破。古腾堡钟通过阅读滚动的 LED 屏幕上的书籍来计时。

时钟的内容来自古腾堡项目，该项目免费发布版权过期的书籍。时钟上的图书馆包括大约两万本这样的书。以每分钟 80 个单词的速度阅读，在接下来的 33 年里，时钟不会重复一段文字。

虽然时钟本身不显示时间，但它与时间同步。两个相同的时钟应该同时显示相同的文本。为了得到时间，[ch00f]首先尝试拆开一个便宜的无线电时钟，它与 NIST 的 60 千赫广播同步。在逆向工程协议取得巨大成功后，来自显示器的杂散射频能量导致了太多的干扰。

随着廉价解决方案的推出，[ch00f]为一个 [Adafruit GPS 模块](http://www.adafruit.com/products/790)建立了一个定制突破，并使用它来获得时间。这是他的第一个射频板，但效果很好。

书籍被加载到 SD 卡上的 FAT 文件系统中，【ChaN】的 [FatFS](http://elm-chan.org/fsw/ff/00index_e.html) 用于解释文件系统。然后，一个微控制器以恒定的速率将文本发送到显示器上的一个串行端口，他侵入了这个端口。

这个项目是艺术和电子的巧妙结合。休息之后留下来观看视频概述。

[https://www.youtube.com/embed/VzwOOGP4DLs?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/VzwOOGP4DLs?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)