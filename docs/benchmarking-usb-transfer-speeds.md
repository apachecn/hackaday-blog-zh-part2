# 基准测试 USB 传输速度

> 原文：<https://hackaday.com/2013/06/03/benchmarking-usb-transfer-speeds/>

![boards](img/27181b65a342a08c326d340f6830298d.png)

Teensy 系列微控制器开发板的创造者[Paul Stoffregen]注意到最近有许多项目驱动巨大的 LED 阵列，他决定研究微控制器开发板从计算机接收数据的速度。当然，每秒更多的位意味着更多的 glowey LEDs，所以他的基准测试努力肯定会受到任何计划一些大规模微控制器项目的人的欢迎。

[Paul]测试的微控制器包括 Teensy 2.0、Teensy 3.0、Leonardo 和 Due Arduinos 以及 Fubarino Mini 和 Leaflabs Maple。这些都是在 Linux ( Ubuntu 12.04 live CD)、OSX 狮子和 Windows 7 上测试的，都运行在 2012 年的 MacBook Pro 上。当不考虑 Teensy 2.0 和 3.0 时，测试结果正如你所料:更快的设备每秒能够接收更多的字节。然而，当青少年被抛入其中时，结果发生了巨大的变化。Teensy 2.0 采用与 Arduino Leonardo 相同的微控制器，能够超越除 Teensy 3.0 之外的所有主板。

[Paul]还努力对他使用的不同操作系统进行基准测试。底线是，如果你一次传输大量的字节，你使用哪个操作系统真的无关紧要。对于传输少量数据，你可能想用 OS X，Windows 传输单字节很糟糕；每次传输一个字节时，Windows 只能管理 4kBps。同样的任务，Linux 和 OS X 分别管理大约 53 和 860(！)kBps。

所以你走吧。如果你正在构建一个巨大的 LED 阵列，请在 MacBook 上使用 Teensy 3.0。当然[Paul]将他的基准测试的所有代码都开源了，所以可以随意复制这个实验。