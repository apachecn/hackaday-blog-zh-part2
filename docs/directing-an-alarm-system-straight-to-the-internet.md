# 将警报系统直接连接到互联网

> 原文：<https://hackaday.com/2012/10/16/directing-an-alarm-system-straight-to-the-internet/>

![](img/806cab2787dda91528578c53ef45e541.png "alarm")

[Scott]在他的房子里有一个非常好的报警系统——它将为他的报警公司的操作员提供足够的信息，以确定这是火警、盗窃还是只是一只猫在传感器前行走。[Scott]想避开中间人，在手机上接收警报系统的通知。在可靠的 Arduino 和非常酷的电动小精灵的帮助下，他做到了。

[Scott]的构建始于将一个 [Arduino 连接到一个 Raspi](http://www.swblabs.com/?p=770) 来监控报警系统的状态变化。因为报警系统的设计者在报警面板和连接到电话线的部分之间包括了非常有用的四线总线，[Scott]发现接入这些线路并读取当前的报警状态相当容易。

将一个 Raspberry Pi 专用于轮询几个 pin 并通过 WiFi 发送数据的简单任务有点过头了，所以[Scott]拿起了一个[电动 Imp](http://electricimp.com/) Arduino shield 来通过 WiFi 传输数据。在之前，我们已经[和小恶魔一起玩过了，[斯科特]很难想出一个更干净的方案来把他的警报监视器放到互联网上。](http://hackaday.com/2012/09/04/hands-on-with-the-electric-imp/)

现在[斯科特]有了一个非常整洁的警报监视器，可以直接向他的手机发送更新，不需要中间人。一个非常整洁的建筑，一个非常酷的 WiFi 设备的出色使用。