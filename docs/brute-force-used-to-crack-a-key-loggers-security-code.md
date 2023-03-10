# 暴力破解键盘记录器的安全代码

> 原文：<https://hackaday.com/2012/10/23/brute-force-used-to-crack-a-key-loggers-security-code/>

![](img/4e3f36ba6892a2feb075162b40df5945.png "brute-forcing-attacking-a-USB-keylogger")

这张图片右侧插入的 USB 设备是在属于一名高级管理人员的公司计算机的键盘和 USB 端口之间找到的。公司雇了 Brad Antoniewicz 来弄清楚这是什么，以及它可能造成了什么样的损害。他最终用暴力破解了解锁码来访问设备，但在此之前他采取了一些谨慎的措施。

从设计和位置来看，硬件最有可能是一个键盘记录器，在互联网上搜索了一番后，[Brad]和他的同事订购了他们认为是同一型号的设备。他们想要一个来测试，然后才开始真正的目标。插入时，记录器不会枚举。取而代之的是，它充当一个通道，跟踪击键，同时监听三键解锁码。[Brad]为 Teensy 微控制器写了一个程序，它可以暴力破解所有的组合。他做了一件好事，因为其中一个组合是制造商硬连线的设备擦除代码。在修改程序以避免擦除代码后，他成功解锁了恶意设备。休息后的视频中有对这一过程的解释。

[https://www.youtube.com/embed/SQgOGTyQw1s?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/SQgOGTyQw1s?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)