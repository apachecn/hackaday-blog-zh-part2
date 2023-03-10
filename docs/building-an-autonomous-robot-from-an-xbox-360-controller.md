# 从 Xbox 360 控制器构建自主机器人

> 原文：<https://hackaday.com/2012/07/20/building-an-autonomous-robot-from-an-xbox-360-controller/>

![](img/30651cc0d3771ef7de658d754d683a6e.png "Build-a-robot-from-an-xbox360-controller")

哇，令人惊讶的是[卡尔]能够使用 Xbox 360 控制 PCB 作为他的机器人的基础来构建[。他的论坛帖子只是触及了构建的表面，但他链接到了一个 PDF 文件，其中有完整的细节。](http://www.dsprobotics.com/support/viewtopic.php?f=61&t=350&p=952#p952)

这种构建基本上是将传感器和替换电机连接到控制板…就是这样！一些距离传感器连接到左右触发器的模拟输入。触须使用几个焊接在控制器按钮垫上的叶片开关。电机是齿轮替代品，使用与隆隆电机相同的连接器。

这个想法是控制器通过 PCB 上的无线电连接到 PC。连接完成后，PC 软件可以读取所有传感器的数据，并相应地驱动电机。使用像 RPi 这样的单板解决方案来消除对远程 PC 的需求也是非常容易的。但这是一个奇妙的开始，是我们以前从未考虑过的方法。休息之后，看看小家伙在房间里走动的视频。

[https://www.youtube.com/embed/1xGA5bDD-Ug?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/1xGA5bDD-Ug?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)