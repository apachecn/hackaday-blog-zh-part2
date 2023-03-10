# 面包在线是物联网的面包机

> 原文：<https://hackaday.com/2015/07/07/bread-online-is-a-bread-maker-for-the-internet-of-things/>

西马其顿大学的一名工程系学生刚刚为越来越多的互联网设备添加了另一种设备。[Panagiotis]决定改装一台现成的面包机，使其能够通过互联网进行远程控制。

[Panagiotis]不得不移除这个设备几乎所有的原始控制电路。原来的控制器换成了 Arduino Uno R3 和以太网屏蔽。温度传感器也需要更换，因为[Panagiotis]找不到任何描述原件规格的官方文件。幸运的是，加热元件和搅拌电机能够重复使用。

机箱上钻了几个孔，为以太网连接器和 USB 连接器腾出空间。两个继电器用于允许 Arduino 打开和关闭加热元件和混合器电机。面包机的前面板上有一个简单的液晶显示屏和几个控制按钮。为了不让它们被浪费掉，它们也被连接到 Arduino 上。

Arduino 面包机可以通过运行在独立服务器上的网站进行控制。该网站是用 PHP 编写的，在 Apache 上运行。它有一个简单的界面，允许用户指定几个设置，包括多少面包是熟的，以及希望面包的黑暗。然后，用户可以安排面包机启动。在线面包还带有“离线”模式，这样它就可以在本地使用，而不需要电脑或网络浏览器。请务必查看下面的视频演示。

[https://www.youtube.com/embed/hoTtp7hwVzE?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/hoTtp7hwVzE?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[谢谢米纳斯]