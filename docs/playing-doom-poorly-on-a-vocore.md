# 在 VoCore 上玩 Doom(很差)

> 原文：<https://hackaday.com/2014/10/19/playing-doom-poorly-on-a-vocore/>

去年 5 月，有一则平淡无奇的消息称，一些公司正在利用 20 美元无线路由器中的片上系统，用它们制作开发板。第一个是 VoCore，Indiegogo 为物联网推出的 360MHz CPU，8MB 闪存和 32MB RAM 封装在一平方英寸的 PCB 中。既然 Indiegogo 的奖励正在走向世界各地的工作台，有人得到*厄运*在其中一个上运行只是时间问题。

在 VoCores 的第一次运行中修复了一些设计缺陷后，[Pyrofer]做了一些你会在运行 Linux 的小系统上做的事情——流媒体视频的网络摄像头，播放互联网广播的 USB 声卡，以及 OpenWrt 做的正常事情。

他的好奇心得到满足后，[Pyrofer]转向了更深奥的建造。用 Sparkfun 的彩色液晶显示器，[他得到了一个运行](https://www.youtube.com/watch?v=sncQPuO8lLE)的 NES 模拟器。请注意，这都是通过硬件 SPI 实现的。简单的 2D 图形已经足够酷了，但是所有低性能计算机的标准图形测试当然是*。*

游戏运行，但只是勉强。尽管如此，[Pyrofer]对 VoCore 还是很满意，通过对 SPI 做更多的工作，并给他的小系统带来一个帧缓冲区，他可能会有一个整洁的便携式*Doom*机器。