# 魅族 MX 使用总线盗版的根源

> 原文：<https://hackaday.com/2012/07/13/meizu-mx-rooted-using-the-bus-pirate/>

![](img/a7f7286e2c0e4ddc445c25b1a71c6eaf.png "meizu-mx-rooting")

令人惊讶的是，对于一些真正强大的智能手机来说，这些电路板竟然如此之小。例如，这款魅族 MX Android 手机的主板尺寸很小，只有手机抵达时复杂的包装才能让它相形见绌。[Adam Outler]打开了设备的包装。但对他来说，这意味着拆除所有的组件，并使用一个总线盗版软件来破解设备。

在休息后的视频中，他坦率地向我们展示了利用这种硬件需要做些什么。您可能会被这些命令吓到，他会一个字符一个字符地大声读出来，但是仔细观察，您会发现它们真的是非常常见的函数。

他的寻根之旅始于阅读主处理器的数据手册，寻找 USART 参数。有了这些信息，他将他的总线盗版器接地，然后在重启时探测电路板上的各个测试点，直到串行数据开始在屏幕上滚动。他找到了 USART 线路，并在上面焊接了一个分接头，这样他就可以在重新组装手机后使用它了。

在那里，他使用总线盗版与电路板的终端合并，然后使用 Android 调试桥重启手机。一旦它启动，Bus Pirate 终端窗口就位于根提示符下(许多公司禁用了这一功能，但[Adam]很幸运)。他将内部文件系统重新挂载为可重写的，然后使用 ADB 将 Linux 替代用户(su)命令推送到设备上，因为 Superuser.apk 程序需要它。这是下一个要安装的东西，一旦安装完成，他就正式拥有了根。

[https://www.youtube.com/embed/WxN0nGfAjUA?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/WxN0nGfAjUA?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)