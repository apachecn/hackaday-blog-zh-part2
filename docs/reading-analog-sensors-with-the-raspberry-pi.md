# 用 Raspberry Pi 读取模拟传感器

> 原文：<https://hackaday.com/2012/07/28/reading-analog-sensors-with-the-raspberry-pi/>

[![](img/d8c9cbe2cf53e5ea53f4b5b24a737bdc.png "raspi")](http://hackaday.com/wp-content/uploads/2012/07/raspi.jpeg)

Adafruit 刚刚发布了一个关于用树莓 Pi 读取模拟传感器的精彩教程。这是一个很好的演练，可以应用于你的下一个 Raspi 项目，以及任何你只需要*多一个*模拟输入的项目。

早些时候，Adafruit [的人发布了一个教程](http://learn.adafruit.com/reading-a-analog-in-and-controlling-audio-volume-with-the-raspberry-pi),介绍如何使用带 Raspi 的 [MCP3008](https://www.adafruit.com/products/856) ADC 直接读取模拟值。不过，有时你不需要 8 路模拟输入和一个 12 位 ADC 来启动项目。Adafruit 的指南介绍了如何在不使用 ADC 的情况下读取模拟值，它依赖于连接在数字输入和地之间的一个 1μF 陶瓷电容。通过将传感器线拉高一到两毫秒，电容会根据模拟传感器的值以不同的速率充电。

是的，这只是一个 RC 定时电路，但鉴于 Raspi 没有模拟输入，我们认为本教程可以帮助一些人。