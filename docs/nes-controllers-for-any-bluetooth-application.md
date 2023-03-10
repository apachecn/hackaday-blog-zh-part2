# 适用于任何蓝牙应用的 NES 控制器

> 原文：<https://hackaday.com/2012/06/01/nes-controllers-for-any-bluetooth-application/>

![](img/1d0c843119a5689a900ae78e0ab9b21c.png "dead-nes-host-bluetooth-translator")

[Dustin Evans]想用他原来的 NES 控制器玩模拟游戏。问题是他不想改变传统的硬件。他的解决方案是使用一个死 NES 的连接器和外壳来构建一个蓝牙转换器，它可以与任何 NES 控制器一起工作。

这里他展示的是 NES 原作被挖空的一半。虽然主板不见了，但是控制器的连接器还在。它们被重新连接到一个 Arduino 板上，这个板上有一个 BlueSMiRF 调制解调器。Arduino 获取控制器命令，并发送给蓝牙连接另一端正在监听的任何设备。他还计划在机箱中增加几个 SNES 端口，这样那些未改变的控制器也可以使用。

在广告之后的视频中,[Dustin]带领我们完成了硬件设置。然后，他演示了如何将该设备与 Android 手机配对，并用图中的控制器玩一些模拟器。

[https://www.youtube.com/embed/gbKzwYtoacM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/gbKzwYtoacM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)