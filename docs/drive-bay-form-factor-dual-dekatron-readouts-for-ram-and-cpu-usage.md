# 针对 RAM 和 CPU 使用情况的硬盘托架外形双 Dekatron 读数

> 原文：<https://hackaday.com/2013/07/26/drive-bay-form-factor-dual-dekatron-readouts-for-ram-and-cpu-usage/>

![optical-drive-dual-dekatron](img/05066eaf6640e181a35bc3c6338757e6.png)

上面看到的两个圆形显示器是内置在光驱外壳中的[de katron。[马特·西尔维斯特]在易贝找到了一些不同类型的管子。他蚀刻了自己的驱动程序，并用 Arduino 控制它们。几个月后，他决定重新审视这个项目，看看它是否能作为一个 CPU 和 RAM 使用计量器。](http://hyperneuron.blogspot.com/2013/07/dekatron-pc-status-display.html)

这些电子管需要高电压才能让霓虹显示器发出明亮的光。这引起了一些人对 PC 内部电压电平以及电源可能引入的噪声的担忧。为了解决这些问题，[Matt]拆除了一个旧的光驱，用它的外壳来物理隔离电路，用一些光隔离器来保护逻辑连接。他的驱动板使用运行 Arduino 引导程序的 ATmega328。它使用 FTDI USB 转串行电缆连接到 PC。这使得将性能数据推送到显示器变得轻而易举。它还有一个好处，就是允许他不用打开外壳就能对芯片重新编程。

如果你在自己的项目中找不到这样的管子，可以考虑用[冒充](http://hackaday.com/2010/09/03/the-spindicator/)。

[https://player.vimeo.com/video/70706738](https://player.vimeo.com/video/70706738)