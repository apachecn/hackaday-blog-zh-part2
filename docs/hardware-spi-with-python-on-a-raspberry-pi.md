# Raspberry Pi 上的 Python 硬件 SPI

> 原文：<https://hackaday.com/2013/01/06/hardware-spi-with-python-on-a-raspberry-pi/>

虽然 Raspberry Pi 非常支持 I2C 总线，但许多非常酷的芯片——包括几乎所有 ATtiny 和 ATmega 微控制器的系统内编程器——都使用 SPI 总线。[Louis]发来了一篇关于如何在他的 Raspi 上获取硬件 SPI 的教程，尽管目前还很有限，但这是朝着正确方向迈出的一步。

之前，[Brian Hensley]发布了一个使用 Raspi 的 Linux SPI 驱动程序的教程。[Louis]想在 Python 中使用 SPI，所以他在 spidev.c 文件中添加了一个 C 扩展名(此处[可用](https://github.com/lthiery/SPI-Py))，允许他打开 SPI 连接、初始化、传输和关闭连接。

将 Arduino 连接到他的 Arduino 的 MOSI、MISO 和 SCK 引脚后，[Louis]能够通过 spi 总线从他的 Raspi 传输数据。应该注意的是，电平转换器在这里确实是一个好主意，但是如果有人想将 AVRDude 移植到 Python，这是一个很好的项目。