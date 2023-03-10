# 从头开始构建的无线 IPod 充电器

> 原文：<https://hackaday.com/2012/05/10/wireless-ipod-charger-built-from-scratch/>

![](img/81fe5cebef14b061b96b4dfc45c8c94a.png "Wireless-Power-Charger")

尽管明显使用了大量的电线，这个项目实际上是一个无线充电系统。[Jared]建造它是为了探索感应转移能量背后的概念。一个白色线圈上的交流电会在另一个线圈上感应出电流。然后对其进行整流和调节，以用作 5V 充电器。在这种情况下，它为他的 iPod 供电，但任何 USB 设备都应该与该设置一起工作。

发射器使用旧笔记本电脑的电源作为电源。一些滤波和几个 MOSFETS 负责在发射线圈上产生交流电流。接收线圈给桥式整流器供电。在文章中，该电压被馈送到 7805 调节器，以提供稳定的 5V 输出。然而，在休息后的视频演示中，[Jared]展示了他在改进电路中使用的升压转换器。这样，如果电压由于线圈排列不当而下降，它仍能提供稳定的输出。

我们已经看到了同样的线圈概念用于给手机增加无线充电功能。

[https://www.youtube.com/embed/MDSYJowwFWM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/MDSYJowwFWM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[通过[使](http://blog.makezine.com/2012/05/08/wireless-ipod-charger/)