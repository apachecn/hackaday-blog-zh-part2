# SLDongle:不断赠送的微控制器礼物

> 原文：<https://hackaday.com/2014/01/24/sldongle-the-microcontroller-gift-that-keeps-on-giving/>

成为[kiu]的同事之一一定很棒。有些人在工作时分发巧克力或压力球作为圣诞礼物，但[kiu] [制作了一堆 SL 加密狗，向他的同事介绍微控制器的世界](http://www.schoar.de/tinkering/sld/)。

这些加密狗基于 atmega 88 pa T1，在三个层次上为每个人提供服务。不需要经验的选择是将其插入 USB 端口，欣赏灯光秀序列。如果你知道足够的危险，你可以使用[kiu]的 sldtool for Linux 或 Mac 从 USB 主机远程控制 led。他最初包含了可视化 CPU 利用率的例子，最终添加了基于 Ruby 的下一趟出站列车在附近 站的出发倒计时。

如果你够 1337，你可以通过 USB 闪存自己的 C 或汇编代码。在开机过程中按住按钮可以让您将加密狗用作 [USBasp](http://www.obdev.at/products/vusb/usbasploader.html) ，这样它就可以以 avrdude 闪烁。[kiu]说 bootloader 不能通过软件解锁，理论上是无法破解的。休息后留下来看完整的演示。

 [https://www.youtube.com/embed/AcsKuC5ylPQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/AcsKuC5ylPQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[谢谢，小九]