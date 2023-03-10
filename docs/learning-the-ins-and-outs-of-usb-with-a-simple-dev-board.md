# 使用简单的开发板了解 USB 的来龙去脉

> 原文：<https://hackaday.com/2012/08/28/learning-the-ins-and-outs-of-usb-with-a-simple-dev-board/>

![](img/323dab61b8d8526a1bbf4ca2bfea849b.png "Usb")

我们无法计算我们在 Hackaday 上看到的带有 USB 端口的项目数量。不幸的是，这些构建中的大多数——从 RepRap 控制器到无线数据记录器——都没有使用 USB 提供给它们的全部功能。[Ben]想出了一个非常酷的 USB 分线板,它可以让你用一个便宜的东西探索 USB 协议。

不是依赖 FTDI 芯片或通过 USB 管道发送串行数据，Ben 的项目是对他的 USB 设备编程书籍的硬件补充。他的硬件板非常简单，只有一个 ATtiny 2313、一个 USB 端口和一些其他组件，但允许[Ben]通过试验板上的八个引脚接收数据，并通过 USB 发送到计算机。

[Ben]不久前送来了他的[USB 数字 8 控制器](http://www.fysnet.net/figure_eight.htm)，这是一块根据通过 USB 接收的数据显示数字 0 到 9 的板。除了学习 USB 如何工作之外，这是一个真正无用的构建，但如果你想为自己的 USB 设备编程，这是一个极好的工具。