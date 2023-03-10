# 轻松实现双向蓝牙通信

> 原文：<https://hackaday.com/2013/07/08/two-way-bluetooth-communication-made-easy/>

很难想象有比遵循本指南更简单的方式来使用蓝牙在 Android 设备和 Arduino 之间建立通信。在试验板的中央，你可以看到廉价且无处不在的 HC-05 蓝牙模块。我们自己拿起其中的一个，我们可以证明，在打开包装并把一个拿在手中后，你可能会突然想到“我从哪里开始？”难题。如果你有一个 Android 手机和一个 Arduino，你就从这里开始，然后有条不紊地一次替换等式的一边，直到你自己的项目有了蓝牙组件，你实际上明白了它是如何工作的。

该项目的硬件由两部分组成。蓝牙模块需要 3.3v 逻辑电平，因此需要考虑这一点。上图显示了进行转换的缓冲芯片，但接线柱上的 Fritzing 原理图使用了分压器。软件方面包括一个 Arduino 草图和一个 Android 应用程序。检查屏幕上的所有控件。通过双向通信和一系列已经配置好的命令，这应该可以让您快速启动并运行几乎任何可能的项目。

需要注意的一点是，这些 HC-05 设备有不同的固件。想了解更多关于这个项目的信息，请看这个项目。

[https://www.youtube.com/embed/USeZd9jthZM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/USeZd9jthZM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)