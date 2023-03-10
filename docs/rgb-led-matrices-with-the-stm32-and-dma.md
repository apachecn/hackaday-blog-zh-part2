# 采用 STM32 和 DMA 的 RGB LED 矩阵

> 原文：<https://hackaday.com/2015/01/05/rgb-led-matrices-with-the-stm32-and-dma/>

几年前，[Frans-Willem]买了几块 RGB LED 面板。10 个 32×16 面板是大量的 led，驱动所有这些面板需要一些足够强大的硬件。他尝试用 FPGA 开发板工作，但那没有足够的内存用于 24 位颜色。微控制器 du jour——TI stellar is——无法在不闪烁的情况下获得超过 16 位的颜色。有了一堆发光二极管，但没有办法驱动它们，[Frans-Willem]将面板放在某个地方的盒子里，等待它们可以被充分利用的那一天。

当[Frans-Willem]通过 F1 发现板推出 STM32 系列芯片时，这一天终于到来了。在寻找一些电子玩具来使用这个板时，他偶然发现了 led 面板，并再试了一次。结果非常壮观，33 位颜色，动画通过无线网络在路由器上播放。

有问题的面板是 HUB75 LED 面板。在 32×8 面板中，有六个数据引脚，每种颜色两个，四个行选择引脚和三个控制引脚。行选择引脚选择在任一时刻哪一行像素是有效的。以足够快的速度在它们之间循环，看起来它们好像是同时开启的。控制引脚的工作方式非常类似于移位寄存器的控制引脚，数据引脚扮演着明显的角色。

在 DMA 和 FSMC 或芯片上的灵活静态存储器控制器的帮助下，实际驱动 led 的代码都在 STM32F4 上完成。该外设负责管理内存中的控制线，因此当您切换写选通时，芯片会将数据线上的内容转储到内存中的特定地址。这是一个产生时钟信号的好方法。

为了将像素发送到这个显示驱动器，[Frans-Willem]使用了一直很受欢迎的 TP-Link WR703N。他原本计划通过 USB 端口发送所有的像素数据，但开销太大，USB 1.1 不够快。通过在路由器上使用 UART 和新的驱动程序以及 OpenWRT 的重新编译版本，这个问题得到了解决。

复制这个项目[的所有软件都可以在 Github](https://github.com/Frans-Willem/LEDMatrixHUB75) 上获得，并且有一个很棒的视频展示了完成的项目可以做什么。你可以看看下面。

[https://www.youtube.com/embed/4_Fv_DULgeM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/4_Fv_DULgeM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)