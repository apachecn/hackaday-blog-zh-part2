# 在英特尔 Edison 上运行 Golang

> 原文：<https://hackaday.com/2014/09/25/running-golang-on-the-intel-edison/>

虽然大多数嵌入式开发仍然是用 C 和/或汇编语言完成的，但有些人正在使用更现代的语言。Gobot 的团队已经成功地让英特尔爱迪生开始运行。

大约五年前出现的 [Go 编程语言](http://golang.org/)可以编译成类似 c 的机器代码，它具有许多现代特性，包括并发性、垃圾收集和包。

我们之前在 Hackaday 上看过 [Edison，甚至还看过](http://hackaday.com/2014/01/07/intel-edison-a-desktop-from-1998-in-an-sd-card/)[详细的硬件](http://hackaday.com/2014/09/10/hands-on-with-the-intel-edison/)。它具有 Quark SoC、蓝牙和 WiFi，非常适合连接设备。

在 Edison 硬件上工作并不特别困难，因为它支持奔腾指令集和 MMX。然而，需要一个库来连接爱迪生的外围设备。Gobot 团队开发了 [gobot-intel-iot](https://github.com/hybridgroup/gobot/tree/dev/platforms/intel-iot/edison) ，这使得使用 GPIO、I2C 和 PWM 变得很容易。

休息之后，团队使用 Go 在 Edison 上演示 PWM。

[https://www.youtube.com/embed/X1ZmNHg0G30?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/X1ZmNHg0G30?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)