# 将 Pi 转换为 IBeacon

> 原文：<https://hackaday.com/2013/12/05/turning-a-pi-into-an-ibeacon/>

![beacon](img/e704fac349fbd4cffa06554626c2ad03.png)

如今，如果你想在当地的自助洗衣店、熟食店或加油站“用 Foursquare 签到”，你需要拿出手机*手动*“用 Foursquare 签到”。好像我们生活在石器时代。苹果的 NFC 竞争对手 iBeacon 通过蓝牙 4.0 改变了这一切。iBeacon 可以自动通知 iOS 和 Android 用户他们在哪里。Adafruit [的凯文·汤森(Kevin Townsend)想出了一个教程，可以把树莓派变成 iBeacon](http://learn.adafruit.com/pibeacon-ibeacon-with-a-raspberry-pi/adding-ibeacon-data) ，完美地告诉你你在树莓派附近的某个地方，还有其他一些很酷的东西。

iBeacon 协议实际上非常简单。基本上，iBeacon 传输的唯一内容是一个 128 位的公司/实体值，以及一个可选的主值和次值(分别用于区分位置和位置内的节点)。将蓝牙 4.0 USB 加密狗插入 Pi 后，安装 [BlueZ](http://www.bluez.org/) 并输入 iBeacon 数据就很简单了。

iBeacon 本身并不真正做任何事情——准确找出你在哪个 Panera Bread 或 Starbucks 的繁重工作就留给了你手机上的应用程序。但是，如果您是一名移动开发人员，这是建立一个非常有用的测试平台的好方法。