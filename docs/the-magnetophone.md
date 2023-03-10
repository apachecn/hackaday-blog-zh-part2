# 磁力电话

> 原文：<https://hackaday.com/2013/12/28/the-magnetophone/>

[![The Magnetophone](img/b386f17b9db88d1f75a2866294884492.png)](http://hackaday.com/2013/12/28/the-magnetophone/magnetophone/)

[磁音器](http://aaron-sherwood.com/blog/?p=1297)是【Aaron Sherwood】最新的电声乐器。这个塔包含 14 根弦和 14 个手动缠绕的电磁铁。通过方波激励每个电磁体，琴弦可以振动产生音乐。

该设备的大脑由一个附着在塔顶的 Arduino Mega 组成。微控制器有 6 个定时器，允许同时播放 6 个音符。一个[开源音调库](https://code.google.com/p/rogue-code/wiki/ToneLibraryDocumentation)被用来产生正确频率的方波。这些方波由基于 LM386 的电路放大，为线圈提供足够的功率来振荡琴弦。通过使用特定频率的方波，可以产生弦的泛音。

这不是我们第一次看到[亚伦]将弦乐和电子结合在一起。他的 [Glockentar](http://hackaday.com/2012/11/28/glockentar-a-guitar-glockenspiel-mashup/ "Glockentar: A Guitar + Glockenspiel Mashup") 使用螺线管来拨动琴弦。然而，这个项目提供了新的可能性，允许振荡率得到精确控制。休息之后你可以看到乐器在演奏。

[https://player.vimeo.com/video/82367702](https://player.vimeo.com/video/82367702)