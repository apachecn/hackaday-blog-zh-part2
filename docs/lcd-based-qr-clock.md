# 基于 LCD 的 QR 时钟

> 原文：<https://hackaday.com/2013/02/28/lcd-based-qr-clock/>

这里有一个新的 QR 时钟概念，它使用了一个 LCD 显示屏。这个概念来自于[ch00f]在他的两个版本的[QR 时钟](http://hackaday.com/2013/02/18/making-a-qr-clock-bigger-cheaper-and-better/)中的工作(两个版本都使用了 LED 阵列)。使用快速响应代码标准对时间进行编码。这个版本每秒生成一个新代码，封装了日期、小时、分钟和秒的信息。如果你看左边的图片，你会注意到代码没有居中。休息后看一下视频，你会发现这是因为它像屏保一样在液晶显示器上跳动。再看一会儿，你会看到右图中显示的迷幻效果。

PIC32 驱动显示器。它连接到一个 DCF77 无线电模块，为系统提供原子钟数据。彩色等离子效果用于显示设备何时锁定无线电信号。

[https://www.youtube.com/embed/OYGP_k4zEm4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/OYGP_k4zEm4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)