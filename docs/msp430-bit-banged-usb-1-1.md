# MSP430 位碰撞 USB 1.1

> 原文：<https://hackaday.com/2012/12/03/msp430-bit-banged-usb-1-1/>

![msp430-usb-hardware](img/d7d88e80d1cc4122b18646214face3d1.png)

对于使用 MSP430 微控制器的人来说，这是一个相当令人兴奋的发展。[M-atthias]研究出一种在 MSP 430g 2452 上实现 USB 1.1 的方法。他有点搞砸了通信，因为这个硬件通常不支持通用串行总线。这很像使用 AVR micros 的 V-USB 堆栈。

上面看到的测试硬件使用了一个 18Mhz 的晶体来获得恰到好处的时序。由于这最大限度地挤压了芯片，固件用汇编语言编写也就不足为奇了。这仍处于开发的早期阶段，但核心功能已经基本具备，并且已经在几个版本中实现和调试过了。目前，基本功能可以使用低于 2k 的闪存来加载。你可以从[M-atthias'] sourceforge 页面下载 Mecrisp 包。如果你想帮忙测试或开发，将不胜感激。

[via [43oh 博客](http://www.43oh.com/2012/12/usb-v1-1-support-on-the-msp430-launchpad/)