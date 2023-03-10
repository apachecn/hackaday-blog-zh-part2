# BadUSB 的意思是我们都完蛋了

> 原文：<https://hackaday.com/2014/10/05/badusb-means-were-all-screwed/>

其他人有没有感觉到相当可怕的漏洞暴露的频率正在加快？在我们的头顶，有心脏出血，休克，现在这一个。[bad USB 漏洞攻击源于大多数 USB 设备中的“隐形”微控制器](https://srlabs.de/badusb/)。

我们第一次听说它是在八月份参加 DEFCON 的时候。Blackhat 在同一周宣布了这一漏洞，但目前还没有太多信息。现在[演讲已经发布](https://www.youtube.com/watch?v=nuruzFqMgIw)并且[在《大混乱》杂志](http://www.bigmessowires.com/2014/10/04/badusb-and-the-hidden-microcontroller/)上有一篇很好解释的综述文章。

这是如何进行的:所有 USB 设备都依赖微控制器来处理 USB 通信的外围设备。计算机不关心哪个微控制器，即使它想知道也没有办法知道。在这种情况下，统一通信是“不可见的”，计算机关心的是接口和流经它的数据。BadUSB 是一种向该微控制器添加恶意功能的攻击。对电脑来说，这是一个完全正常的功能性 USB 设备，而所有不好的事情都发生在电脑看不到的外设控制器上。

![badusb](img/ccb990237d206e29240f69f76b026e7b.png)

你认为插上每一个 USB 设备有多难？看看下面的视频，看看 19:20 发生了什么。USB 设备枚举并非常快速地建立一个欺骗的以太网连接。您仍然可以通过 WiFi 加载网页，但虚假连接会将数据包转发到第二台服务器。

一旦发现，可以对电脑进行擦除，这种情况就会停止发生；直到你再次插入同样的装置并再次感染。更糟糕的是，因为控制器对计算机是不可见的，所以几乎没有办法扫描被感染的设备。如果你*足够聪明*怀疑 BadUSB，你要花多长时间才能弄清楚是你的鼠标、键盘、u 盘、网络摄像头、扫描仪……你明白了。

[https://www.youtube.com/embed/nuruzFqMgIw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/nuruzFqMgIw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[谢谢 Kuldeep]