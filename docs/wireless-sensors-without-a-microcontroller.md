# 无微控制器的无线传感器

> 原文：<https://hackaday.com/2012/08/05/wireless-sensors-without-a-microcontroller/>

[![](img/ace1735cb135d0beb8bd69cdf9752605.png "sensor")](http://hackaday.com/wp-content/uploads/2012/08/sensor.jpeg)

有一天在网上闲逛时，[Raj]发现了一对由 Dorji 应用技术公司制造的非常酷的射频发射器和接收器。这些模块 DRF5150S 和 drf 4432s——除了模拟和数字输入引脚的输入之外，工作方式与任何其他 ISM 频段发射机接收机对一样。整理一份使用这些无线电模块的教程，如果您的下一个项目需要一个非常简单的无线连接，这将是完美的选择。

[Raj]的使用指南[Dorji 传感器模块](http://www.dorji.com/pro/Modules/Wireless_sensor_module.html)显示变送器有两种工作模式。第一种模式是简单的数据发送器，通过 UART 连接与微控制器相连。“传感器”模式不需要单独的芯片；片上 STM8L151 微控制器读取两个引脚上的模拟值，并通过无线将其发送至 DRF4432S 接收器模块。

通过 Dorji 发布的应用程序将发射器编程为无线传感器后，[Raj]将发射器插入带有电池和数字温度计的试验板。接收器模块插入 USB -> UART 模块，数据从终端中的传感器下拉。

[Raj]在 Processing 中编写了一个小应用程序来显示来自传感器的数据。他有一个奇妙的动画温度计，显示传感器的温度读数，电池电压和无线信号的强度。非常简单，如果你需要一个简单的方法来建立一个无线传感器，这是一个非常有用的教程。