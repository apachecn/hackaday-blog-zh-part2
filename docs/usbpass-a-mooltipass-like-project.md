# USB pass——一个类似 Mooltipass 的项目

> 原文：<https://hackaday.com/2014/01/01/usbpass-a-mooltipass-like-project/>

[![](img/5b7eed27b8b6f3cda3d2bfe41599e085.png)](http://hackaday.com/wp-content/uploads/2013/12/reva_built.png)

在我们根据 Hackaday 系列开发的[中，一些读者可能记得我们写的一句话:“如果一个人的想法还没有进入市场，它要么是完全愚蠢的，要么是人们已经在努力了”。嗯，[乔希]无意中提到，在最近加入我们的](http://hackaday.com/tag/developed-on-hackaday/)[谷歌小组](https://groups.google.com/forum/#!forum/mooltipass)后，他也在研究一个[离线密码管理器](http://sroz.net/projects/usbpass/)。与 Hackaday 开发的平台类似，USBPass 通过 USB 连接到计算机，并被检测为 HID 键盘。从上图可以看出，它使用的元件非常少:一个 ATMega32U2，一个 USB 连接器，三个按钮和几个无源芯片。

总共 20 个密码可以存储在微控制器的存储器中，可以由平台使用按钮“键入”。USBPass 固件基于 [LUFA](http://www.fourwalledcubicle.com/LUFA.php) USB 堆栈，其中【乔希】添加了 HID 报告功能，允许从他的桌面应用程序传输数据。后者使用 Linux/Windows/OS X [HID API](http://www.signal11.us/oss/hidapi/) 库，因此很快就可以将他的软件移植到其他操作系统上。所有的项目资源都可以在 [GitHub](https://github.com/jnwatts/USBPass) 上找到，而【乔希】目前正在进行 B 版本的工作，其中将包括一个有机发光二极管屏幕。