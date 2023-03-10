# 在两个 TI 计算器之间发送无线文本

> 原文：<https://hackaday.com/2014/04/27/send-wireless-txt-between-two-ti-calculators/>

![TI calculators with wireless circuitry](img/119cf039b5923d5f65263a8cb01e3afc.png)

一天，当坐在康奈尔大学教室里的课堂上时，[威尔]和[迈克尔]想到通过他们的德州仪器计算器互相发送文本消息该有多酷。用串行电缆连接两个串行端口是不可能的。因此，他们决定开发一种适用于 TI-83 和 TI-84 计算器的无线链路。

该系统由一对 ATmega644 和两个 [Radiotronix RF 模块](https://www.linxtechnologies.com/en/products/modules/dts-rf-transceiver)供电，这两个模块在两个串行端口之间建立了无线链接。串行端口是 3 线端口，可用于多种用途，包括充当[电视输出端口](http://hackaday.com/2010/10/30/tv-out-for-ti-calculators-using-the-link-port/)。[Will]和[Michael]对端口协议进行了逆向工程，并出色地解释了所有细节。因为它们处理的是最低层的物理协议，所以它们不需要处理更高层的协议，如校验和、报头包等。

休息过后，请务必留下来观看该项目的视频。对于今天的标准来说已经相当慢了。如果你对如何加快速度有什么想法，一定要在评论里让大家知道。

[https://www.youtube.com/embed/lbqcD5elNM4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/lbqcD5elNM4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)