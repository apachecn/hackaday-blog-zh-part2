# Webmote:用基于网络的遥控器控制任何东西

> 原文：<https://hackaday.com/2012/12/14/webmote-control-anything-with-web-based-remote/>

![control-anything-from-the-web](img/b92543c058c18e58fb1cbfc87dc2ffac.png)

我们已经看到了很多让你从智能手机上控制所有设备的项目。但是这个基于网络的通用远程控制系统看起来是我们见过的最通用的。该项目被称为 Webmote，因为控件是作为一个网络界面提供的，所以你不局限于说一个 Android 设备。可以通过选择要使用的按钮以及将它们放置在显示屏上的什么位置来定制 UI。你可以通过观看[这张 G+专辑](https://plus.google.com/u/0/photos/114801052085717416954/albums/5244814407639128177)来感受一下。多亏了一个附加系统，设置变得简单了一些，这个附加系统为控制 XBMC 等常见事情提供了预定义的布局。

上面看到的硬件是 Webmote 的业务端。这是一个 Arduino，带有红外接收器、红外 LED 和 XBee 模块。对于常见的家庭娱乐设备，您可以使用红外接收器向系统输入您的代码。红外 LED 用于传输这些代码，Xbee 使您能够控制 X10(家庭自动化)设备。目前的设置要求硬件通过 USB 连接到服务器，但设置某种类型的无线替代方式应该不难。