# FPGA 上的 LVDS 使得重复使用笔记本电脑液晶显示器之类的东西成为可能

> 原文：<https://hackaday.com/2012/10/03/lvds-on-an-fpga-could-make-it-possible-to-reuse-laptops-lcds-and-the-like/>

![](img/3857c517314ae70e01fc1d96b6004c2b.png "LVDS-Display-Controller-V1.0")

在互联网上搜索一下，你会发现一堆论坛帖子在问如何从一台坏了的笔记本电脑上驱动液晶显示屏。答案总是没有办法做到这一点。这是因为它们中的大多数使用低压差分信号协议，这是业余爱好项目中使用的硬件所不具备的。但这块板的出现可能预示着事情即将发生变化。我们不想让你抱太大希望。这不是一个开源项目，但它是一个硬件，可以让你习惯使用的 8 位、16 位和 32 位微控制器使用 LVDS。

这是[托马斯·叶斯柏森]为一个客户做的一个项目的衍生物。它使用 FPGA 来实现高像素 LCD 显示器使用的 LVDS 标准。它包含足够的内存来容纳一个完整的帧缓冲区，并包含摩托罗拉-8080 通信标准。[Thomas]在休息后的视频中详细描述了该设置的工作原理。视频中演示大约在 7:30 开始，由 STM32 F4 发现板驱动显示屏。

[https://www.youtube.com/embed/1Wpw8u6kqO8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/1Wpw8u6kqO8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)