# 用 FPGA 驱动 PSP 屏幕

> 原文：<https://hackaday.com/2012/06/18/driving-a-psp-screen-with-an-fpga/>

![](img/f07f63a87431e57ea7a97a8a5c679abb.png "driving-psp-screen-with-fpga")

下面是[FlorianH]用 FPGA 驱动 PlayStation 便携屏幕的设置。他使用 DE0-Nano 板来完成这项工作，首要任务是建立一种连接两者的方法。他在蚀刻自己的分线板方面做得很好，有些痕迹不到 10 密耳厚。焊接屏幕的连接器是一个挑战，他分享了几个过程的图片供您欣赏。

一切就绪后，他只用几行代码就启动了它，绘制了一个测试模式。从那时起，它就开始[构建一个更强大的驱动程序](https://sites.google.com/site/fpgaandco/de0-nano-niosii-lcd-driver)。[FlorianH]向我们提到，在广泛使用 8 位微控制器之后，他才刚刚开始学习 FPGAs。他一直在他的网站上记录他的工作，并发现自己经常引用他自己的材料，所以记住他是如何做事情的。我们的间接享受是这种习惯的一个意想不到的(但受欢迎的)结果。