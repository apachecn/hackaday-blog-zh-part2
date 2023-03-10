# 多路 Pi 摄像机

> 原文：<https://hackaday.com/2014/12/19/multiplexing-pi-cameras/>

Raspberry Pi 及其酷炫的摄像头附件是将图像和视频发送到 Intertubes 的绝佳方式，但如果您想要监控多个场景，该怎么办呢？IVPort 可以复用多达 16 个这样的 Raspi 相机模块，为 pi 提供 16 种不同的世界视图和一堆高得离谱的连接到 GPIO 头的电路板。

Raspberry Pi 的 CSI 接口使用从相机到 CPU 的高速数据线来快速获取大量图像数据。另一方面，控制相机使用常规的旧 GPIOs，这种 GPIOs 与标题上的 GPIOs 相同。我们已经看到过[重复使用这些 GPIO 来闪烁 LED](http://hackaday.com/2014/07/24/adding-gpios-to-the-raspberry-pi-with-the-camera-interface/) 的构建，但是使用带有额外相机连接器的分线板，可以使用普通 GPIO 线来代替相机端口 GPIO。

结果是一个可堆叠的扩展板，将相机端口分成两部分，允许连接四台 Raspi 相机。在上面再叠一块板，你就可以再加四台相机了。总共四个这样的板可以堆叠在一起，多路复用 16 个 Raspberry Pi 摄像机。

至于显而易见的“为什么”问题，你可以用十几台电脑控制的相机做一些有趣的事情。显而易见的选择是子弹时间相机钻机，这是这块板应该能够做到的，因为它在通道之间切换的时间只有 50 纳秒。下面的视频。

[https://www.youtube.com/embed/rhP1r1i4D7o?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/rhP1r1i4D7o?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/vbtqg0oY-E4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/vbtqg0oY-E4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)