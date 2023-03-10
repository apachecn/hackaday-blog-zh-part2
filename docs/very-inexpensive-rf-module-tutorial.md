# 非常便宜的射频模块教程

> 原文：<https://hackaday.com/2012/08/19/very-inexpensive-rf-module-tutorial/>

![](img/55cb5b8a46b28b11549d3a7a1034ab48.png "radio")

比方说，你需要一种无线项目的方式，但没有 ZigBee 之类的东西。你可以使用红外线，但它的范围有限，只能在接收器的视线范围内工作。[Camilo] [发送了一个项目](http://candelectronica.blogspot.com/2012/08/contro-remoto-por-rf-con-modulos.html)(西班牙语，[翻译](http://translate.google.com/translate?sl=es&tl=en&js=n&prev=_t&hl=en&ie=UTF-8&layout=2&eotf=1&u=http%3A%2F%2Fcandelectronica.blogspot.com%2F2012%2F08%2Fcontro-remoto-por-rf-con-modulos.html&act=url))通过无线串行连接连接两个设备。作为一个小奖励，他的无线装置足够便宜，可以创建一个由几十个传感器组成的无线网络。

[Camilo]使用 TLP 434 a 发射器/接收器组合来启动他的无线项目。这些小设备只需 5 美元，但如此便宜意味着硬件设计者需要自己开发通信协议。

对于微控制器，[Camilo]选择了 Freescale MC9S08QC，这是我们通常看到的 AVR 或 PIC 的一种令人愉快的重复。在为他的发射器做了一个小板子后，[Camilo]有了一个非常小的遥控器，能够向远程接收器发送按钮按压或其他数据。

休息之后，你可以看到一个简短的演示视频[Camilo],视频中他的无线发射器打开了连接在接收器上的 LED。不幸的是，这个视频是用土豆拍摄的，但所有的原理图和代码都在他的网站上，供您阅读。

[https://www.youtube.com/embed/kuhHdqkhlys?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/kuhHdqkhlys?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)