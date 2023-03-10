# 任天堂光枪改造让它玩基于颜色的游戏

> 原文：<https://hackaday.com/2012/10/02/nintendo-light-gun-retrofit-lets-it-play-color-based-games/>

![](img/0e29b09e904af7d0186a27e330e24778.png "nintendo-light-gun-retrofit")

这款任天堂光枪，又名 Zapper，看起来像一个库存设备。但是往里面看了一眼，发现电路板已经被换掉了。添加了 USB 功能和一些额外的传感器，让他可以使用经典控制器编写自己的游戏。

打开箱子后，他测量了电路板的形状，这样他就可以精确地复制它了。这让他设计了自己的板子，它可以像原来一样直接落入相同的塑料支撑件中。他的电路使用 ATmega8u2 提供 USB 连接，并读取连接的传感器。一个有趣的方面是四条长走线组成的一组走线充当可扩展的 i2c 总线。[CNLohr]这样做是为了以后他可以使用子板添加传感器。在视频之后的演示中，他使用光电二极管作为颜色传感器。这让他可以编写上面看到的基于颜色的游戏，在每一轮中你可以射击不同颜色的目标。

[https://www.youtube.com/embed/gyejLFW_TCg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/gyejLFW_TCg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[via [Reddit](http://www.reddit.com/r/electronics/comments/10dh3l/nintendo_zapper_with_color_light_sensor_and/)