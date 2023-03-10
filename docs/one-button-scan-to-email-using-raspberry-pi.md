# 使用 Raspberry Pi 一键扫描至电子邮件

> 原文：<https://hackaday.com/2013/01/10/one-button-scan-to-email-using-raspberry-pi/>

![one-button-scan-to-email-raspberry-pi](img/76f1fb96b86fb7c7d723b6be984ec7ad.png)

我们遇到过极其昂贵的复印机，它们也可以传真、扫描到电子邮件，而且通常有太多的功能需要列举。[Eduardo Luis]想出了如何使用非常便宜的组件来实现这种办公室魔术。具体来说，他可以[按下一个按钮扫描一份文件，并将其发送到一个电子邮件地址](http://eduardoluis.com/raspberry-pi-and-usb-network-scanner/)。

用户控制 RPi GPIO 头的配线。有一个我们已经提到的按钮，一个红色的 LED 表示“系统忙”，一个绿色的表示“系统状态”。一组脚本监控按钮并驱动 led。当需要扫描时，RPi 使用 scanimage 包捕获一个. PNM 文件，然后将其转换为。JPG，然后用 mutt 软件包通过电子邮件发送。

我们希望看到一个字符液晶显示器和一些更多的按钮添加到设置。这样你可以在不同的收件人之间进行选择(甚至通过传真发送)。而且总是有可能将打印机连接到 RPi 上的另一个 USB 端口，使其也可以作为复印机使用。

你可以在跳跃后观看演示视频。

[https://www.youtube.com/embed/obNpPtNltdU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/obNpPtNltdU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)