# Raspberry Pi 计算模块

> 原文：<https://hackaday.com/2014/04/07/the-raspberry-pi-compute-module/>

Raspberry Pi 集群计算机现在已经过时了，令我们沮丧的是，我们甚至看到 Raspberry Pi 作为几个考虑不周的 Kickstarter 项目的大脑出现。Pi 从来不是为这些应用程序设计的，它有非常奇怪的端口布局和一堆大多数人不需要的头。Raspberry Pi foundation 为普通消费者 Pi 的奇怪布局提供了解决方案:[Raspberry Pi 计算模块](http://www.raspberrypi.org/raspberry-pi-compute-module-new-product/)，这是一个 Raspi 和 4GB 闪存驱动器，无连接器，位于行业标准的 DDR2 SODIMM 模块上。

这不是你可以插入你的笔记本电脑的东西(还没有；这只是一个 BIOS 黑客了，对不对？)，但新的格式确实允许一些非常有趣的项目。所有正常的 Raspi I/O——CSI 和 DSI 端口、USB、HDMI、JTAG——以及一大堆 GPIO 端口——都被分解到一个 I/O 板上进行开发。这个想法是任何人都可以为 Raspberry Pi 开发一个产品，创建一个带有 SODIMM 连接器的定制板，并使用计算模块作为他们项目的大脑。

这款计算模块的 100 片订量价格应该在 30 美元/片左右，将于 6 月上市。目前还不知道 I/O 板的价格，但我们预计很快会出现一些开源扩展板，这样任何人都可以基于计算模块创建一个非常酷的集群计算机。