# 使用蓝牙查找您的钥匙

> 原文：<https://hackaday.com/2012/04/23/finding-your-keys-with-bluetooth/>

![](img/fda021125139feeb01fdf60e0de8a242.png "keys")

[多拉加斯]的妻子总是乱放钥匙。为了解决这个问题，[doragasu]创造了一个小的[蓝牙钥匙链](http://kernelhacks.blogspot.com/2012/04/btkeychain.html)，当手机发出命令时，它能够远程发出警报。

[doragasu]项目的外壳和 LiPo 电池来自一个小相框钥匙链。相框的 LCD 显示器和 PCB 被扔到一边，留待将来的项目使用，电路的设计也开始了。蓝牙蜂鸣器密钥卡基于 MSP430 微控制器，因为它们的功耗要求极低。

在软件方面，[doragasu]建立了一个 J2ME 应用程序，连接到密钥卡，并打开蜂鸣器。他的应用可以移植到任何安卓手机上，版本可以移植到 Windows、OS X 和 iOS 设备上。

它是如何工作的？嗯，[多拉加苏]的妻子有时会忘记给她的钥匙链充电，导致整个项目毫无用处。有想法将设备更新为蓝牙 4.0 低能耗设备，但没有可行的计划。不过，做得很好。休息之后，你可以看看[doragasu]的演练和演示视频。

[https://www.youtube.com/embed/zdn7MZvHQyc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/zdn7MZvHQyc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)