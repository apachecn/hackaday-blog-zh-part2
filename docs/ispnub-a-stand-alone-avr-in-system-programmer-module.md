# ISP nub——独立的 AVR 系统内编程器模块

> 原文：<https://hackaday.com/2014/04/11/ispnub-a-stand-alone-avr-in-system-programmer-module/>

[![](img/df748f416f7883735f77206a3107e532.png)](http://hackaday.com/wp-content/uploads/2014/04/isp.png)

[Thomas]向我们透露了他的最新项目:[一个名为 ISPnub](http://www.fischl.de/ispnub/) 的独立 AVR 编程器模块。在上图中可以看到，它是一个简单的电路板，由一个主微控制器(ATmega1284p)、一个按钮和两个 led 组成。对目标进行编程非常简单，只需连接 ISPnub 并按下按钮。然后使用绿色/红色 LED 显示闪烁的操作成功状态。

ISPnub 从目标电路获得电源，因此不需要外部电源。它在 1.8V 至 5.5V 的宽电压范围内工作。该模块还具有一个编程计数器，可用于限制编程周期的数量。多平台 Java 工具负责将目标 flash 内容嵌入到 ISPnub 主固件中。完整的项目是开源的，所以你可能想查看官方的 [GitHub 库](https://github.com/EmbedME/ISPnub)以获取固件，查看项目页面以获取原理图。