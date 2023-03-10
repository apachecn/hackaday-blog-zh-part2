# 哈利波特定位时钟间谍你的智能手机

> 原文：<https://hackaday.com/2013/02/11/harry-potter-location-clock-spies-on-your-smart-phone/>

![harry-potter-clock](img/983a717bbe8870baf1042a11fe9d00d8.png)

《哈利·波特》系列中的定位时钟是一个非常有趣的破解方式。当然，这并不需要什么魔法，只需要[一套监控手机 GPS 的硬件和一个显示它的钟面](http://www.alastairbarber.com/index.php?post=harry-potter-weasley-clock)。

[阿拉斯泰尔·巴伯]去年年底完成了这座钟的建造，作为圣诞礼物。上面看到的展示使用了一个旧壁炉架时钟，给它一个完美的外观。他用系统已知的各种位置的打印结果替换了钟面，并增加了一个伺服电机来驱动单手。他的硬件选择是基于他手头已经有的东西和可以廉价获得的东西。一体式封装将 Raspberry Pi 板与 USB 宽带调制解调器结合在一起，以确保它具有持久的网络连接([我们过去已经看到使用 WiFi](http://hackaday.com/2012/07/30/magic-clock-locates-your-friends/) 实现了这一点)。RPi 检查手机的 GPS 数据，将其与常用地点列表进行比较，然后将命令推送到 Arduino，Arduino 控制时钟指针的伺服电机。这是一种迂回的做事方式，但我们认为当礼物的新鲜感消失后，所有东西都会被重新利用。