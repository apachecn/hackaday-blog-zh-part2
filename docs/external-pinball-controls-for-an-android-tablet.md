# Android 平板电脑的外部弹球控件

> 原文：<https://hackaday.com/2013/05/12/external-pinball-controls-for-an-android-tablet/>

![android-pinball-controls](img/1ee41da2c4409987f7bed6b3ff818c2c.png)

这个黑客[给 Android 弹球](http://forum.43oh.com/topic/3128-msp430-launchpad-android-pinball/)增加了外部脚蹼控制，这是一个在 Android 硬件黑客攻击中大放异彩的方法。

[Ruben]决定在这个项目中使用 TI Launchpad。MSP430 开发板通过 USB 连接提供串行通信，但这不像找到正确的电缆那么容易。他的平板电脑确实支持 USB On the Go (OTG)，但董事会认为自己是一个 ACM 设备，需要以不同的方式处理。为了让平板电脑与 Launchpad 对话，他为构成每个 Android 操作系统的 Linux 基础编写了一个 CDC_ACM 模块。在这种情况下，该模块是为他的平板电脑模型中的 Allwinner A10 芯片量身定制的，但将他的指南用于其他处理器应该不会太难。

当然，你可以走不同的路线，使用蓝牙连接。我们已经看到一些游戏外设在 Android 设备上使用这种技术。

[https://www.youtube.com/embed/JnktHs1wj08?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/JnktHs1wj08?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)