# 用于 Raspberry Pi、BeagleBone 等的 RF 无线内核模块

> 原文：<https://hackaday.com/2013/06/27/rf-wireless-kernel-module-for-raspberry-pi-beaglebone-and-others/>

![rfm12b-kernel-module](img/7c58197fe2c942ab98e8c89104a66461.png)

如果你在业余爱好电子产品上做过任何无线工作，你可能会认出这部分。绿色 PCB 是 RFM12B 无线板。它们有几种不同的工作带宽，433 MHz 可能是最常见的。它们非常容易与小型微控制器接口，但嵌入式 Linux 板呢？这就是这个项目的重点，它为射频模块构建了一个内核驱动程序。

几块钱就可以自己弄个 RFM12B。配对时，它们非常通用，但许多廉价的无线消费品都在这个频段上工作，因此该板可以用来向无线插座、灯具等发送命令。[Georg]一直在研究比格犬骨，比格犬骨黑和树莓皮。他的软件包允许您构建一个内核模块，将设备的条目添加到 Linux 系统的/dev 目录中。到目前为止，列出的三种板都是受支持的，但如果您有五个可用的 I/O 引脚，那么为其他硬件定制这种引脚应该很容易。

想知道你还能做些什么吗？这将使短信门铃的接收端立即启动并运行。

[https://www.youtube.com/embed/5aeSIBstJS0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/5aeSIBstJS0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)