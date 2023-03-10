# 将电视遥控器用作 HID 鼠标

> 原文：<https://hackaday.com/2012/07/19/use-your-tv-remote-as-an-hid-mouse/>

![](img/49b101e549e03052465862f837f66547.png "tv-remote-as-hid-mouse")

Vinod 的最新项目让他可以将电视遥控器当作鼠标使用。这听起来可能不多，但他用最少的硬件做到了这一点，并最大限度地增加了功能。

他使用 ATmega8 读取遥控信号并提供 USB 连接。通过 V-USB 堆栈,他将该设备枚举为一个 HID 鼠标。一个警告，他使用了来自 [USBasp 程序员项目](http://hackaday.com/2011/08/26/dev-board-from-an-avr-programmer/)的 PID/VID 对。如果你使用那个程序员，你需要卸载驱动程序来让它工作(我们认为这只是在 Windows 机器上有必要)。

使用遥控器上的数字键盘可以向八个方向移动光标。数字 5 位于方向键的中间，所以[Vinod]将其映射为左键单击，而零键则作为右键单击。他甚至通过使用音量按钮来包含滚轮。固件支持光标加速。如果你保持一个方向，光标将开始缓慢移动，然后加快速度。通过单击按钮可以进行微调。休息之后，请看他的演示。

[https://www.youtube.com/embed/94ere__-UV4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/94ere__-UV4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)