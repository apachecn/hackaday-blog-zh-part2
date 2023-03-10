# 从零开始的 7 英寸触摸屏电视遥控器

> 原文：<https://hackaday.com/2014/04/14/a-7-touchscreen-tv-remote-control-from-scratch/>

[杰森]一直想要一个触摸屏电视遥控器。他本可以将一款旧的 Android 平板电脑投入使用，但他想推出自己的系统。[Jason]收集了零件，并且正在[建造他自己的 7 英寸触摸屏装置](http://atomsoft.wordpress.com/2014/04/12/portable-remoteseven-3/)。他从一个 7 英寸的液晶电容触摸屏开始。他从远东供应商 buy-display.com 的 T2 订购了他的显示器。

[Jason 的]特定显示器型号安装在 PCB 上，其中包括显示器和触摸屏的控制器，以及一些内存和粘合逻辑。LCD 控制器板有相当多的跳线来支持多种接口和选项。虽然显示的文档很不错，但[Jason]确实发现了一些错误。在与 buy-display 的技术支持取得联系后，他[编写了一个简单的应用程序](http://atomsoft.wordpress.com/2014/03/26/7-capacitive-touch-lcd/)，该程序根据从下拉列表中选择的硬件接口来确定要设置的跳线。

LCD 解决后，[Jason]仍然需要一个处理器。他选择了德高望重的[微芯片 PIC32MX](http://www.microchip.com/pagehandler/en-us/family/32bit/architecture-pic32mxfamily.html) 系列。这个决定允许他在系统成熟之前，使用一个 [Fubarino](http://fubarino.org/) 用于早期原型，然后切换到他自己的板。[Jason]能够启动并运行一个简单的 GUI，用标准的遥控按钮来控制他的电视和有线电视盒。代码在他的 [Github 库](https://github.com/AtomSoftTech/RemoteSeven)上。

[杰森]最近的工作集中在切断脐带上。他已经从 DC 电源换成了 2600 毫安的 LiPo 电池。点击休息时间，观看[Jason]测试他正在进行的全无线工作。

[https://www.youtube.com/embed/N6ASuMZWNfA?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/N6ASuMZWNfA?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)