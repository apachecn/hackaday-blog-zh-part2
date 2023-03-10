# 需要快速参考美国宪法？6 秒钟怎么样？

> 原文：<https://hackaday.com/2014/03/21/need-to-reference-the-us-constitution-fast-hows-6-seconds-sound/>

![CONSTI2GO-Thibault-Brevet-2](img/03388551e9eecfcf3254293fd36018bc.png)

嗯，除非你确切地知道你指的是什么，否则这将花费你更多的时间，但是这个[聪明的串行收据打印机黑客](http://www.designboom.com/technology/consti2go-receipt-printer-hacked-to-print-the-us-constitution-in-6-seconds-03-13-2014/)将让你在仅仅 6 秒钟内打印整个该死的东西！

受[杰夫·戈登森]委托为他的 [LABRARY.bike](http://labrary.bike/) (字面意思是自行车上的弹出式图书馆)制作，它实际上在 SXSW Interactive 上展示过——有人亲自看过吗？创造它的艺术家兼黑客是[Thibault Brevet]，他给我们带来了 [DRM 椅](http://hackaday.com/2013/03/04/drm-chair-only-works-8-times/)，它只工作 8 次就碎了。

无论如何，这个看起来很酷而且相当可疑的电子管有一根串行线挂在外面，包含一个 Arduino，一个 max232 芯片和一个小型 Li-Po 电池。Arduino 通过 max232 芯片将 TTL 信号转换为 RS-232 与打印机通信。它的顶部有一个按钮，当它连接到打印机时，将通过 ESC/p 语言通过串行接口发送美国宪法。

我们提到它有多快了吗？

[https://player.vimeo.com/video/88304676](https://player.vimeo.com/video/88304676)

一旦你知道了如何与收据打印机沟通，收据打印机会变得很有趣。在那之后，你将会像明天一样浪费收据纸，用这个极其浪费(但是很棒)[的基于打印机的视频游戏！](http://hackaday.com/2011/06/20/receipt-racer-wastes-a-lot-of-paper/)

【谢谢 Itay！]