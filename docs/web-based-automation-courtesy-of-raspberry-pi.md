# 覆盆子 Pi 提供的基于网络的自动化

> 原文：<https://hackaday.com/2013/07/12/web-based-automation-courtesy-of-raspberry-pi/>

![web-based-automation-via-rpi](img/02732113cce09dea8526cad8da2f9bba.png)

这个项目是树莓 Pi 在交互方面超越 Arduino 的一个很好的例子。[Fall dear]提到他曾经使用带有以太网屏蔽的 Arduino 板来为他的项目添加可扩展的交互性。但是这个是[家庭自动化灯项目](http://falldeaf.com/2013/07/the-pi-control-script/)，用的是树莓派。这些概念最终非常相似。但是硬件的成本更低，编码工作也更容易。

不要误解我们，硬件是根本不同的。当您从 Arduino 迁移到 RPi 时，您会丢失一些 I/O 引脚，并且对它们的低级控制也不那么直接。但是你也不必用 c 语言编程，Linux 内核处理底层控制，这意味着你可以用 Python 写你的脚本。因为 Python 是一种解释型语言，所以测试和调试要快得多——不需要刷新新代码，只需再次运行脚本。

该项目使用 RPi GPIO 来驱动使用 WS2801 协议的 led 灯条。该板包括一个网卡，这使得它可以很容易地用作网络服务器。上面看到的智能手机控件是使用 jQuery 从 Pi 提供的。现在有一根电线从灯里伸出来了。但是应该有足够的空间来使用拧入式插座适配器，并隐藏里面的 RPi 和 PSU。

该板仍有足够的能量来驱动其他自动化功能，如充当网络广播服务器。

[https://www.youtube.com/embed/xo-cW8CbB4o?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/xo-cW8CbB4o?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)