# 虚拟触摸屏(3D 超声波雷达)

> 原文：<https://hackaday.com/2014/08/24/a-virtual-touchscreen-3d-ultrasonic-radar/>

![virtualtouch](img/fea1fafaebcadcc309897bdf8f70aa2d.png)

仅仅通过触摸空气就能在屏幕上制作物品是一件不可思议的事情。实现这一点的一种方法是使用四个 HC-SR04 超声波传感器单元，通过 Arduino 将数据传输到 Linux 计算机中。最终的结果是一个可以在家里制作的虚拟触摸屏。

这个设备的软件是由[Anatoly]开发的，他将手势转化为可操作的命令。安装在 Arduino 上的传感器的扫描范围大约为 3 米，超声波装置被修改为以 40 千赫的频率广播模拟信号。正如[Anatoly]在帖子中所说，最初的硬件设计有一些限制。例如，起初，一次只有一个单元在传输，所以 Arduino 无法识别同一个球体上的两个物体。然而，[Anatoly]在博客上更新了第二篇文章,表明一次感应多个物品是可行的。偶尔，在处理钢笔等小件物品时，该系列会很挑剔。但除此之外，它似乎工作得很好。

其他技术规范可以在[Anatoly]的博客上找到，系统工作的视频可以在休息后看到。

[https://www.youtube.com/embed/SpZ_CqVk3e8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/SpZ_CqVk3e8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/MPAPJX-6rJ4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/MPAPJX-6rJ4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

【感谢提示 joo！]