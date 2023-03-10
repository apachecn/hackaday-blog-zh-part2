# 一场盛大的水果树莓派对

> 原文：<https://hackaday.com/2012/08/18/an-adafruit-raspberry-pi-extravaganza/>

![](img/733d32d374653200a6dea69f00921e00.png "Raspi")

Adafruit 的工作人员正忙得不可开交，将他们的一些非常酷的板带到 Raspberry Pi 平台上。以下是过去几天收到的一些信息:

#### 16 个伺服系统太多了

伺服系统需要一个 PWM 输出，但 Raspi 只在一个 GPIO 引脚上提供硬件支持；当然不足以建造一个巨大的，能铲平城市的机器人。[凯文]在 Adafruit [组装了一个 tutoria](http://learn.adafruit.com/adafruit-16-channel-servo-driver-with-raspberry-pi/overview) l，用于使用[这个 16 通道伺服驱动器](http://adafruit.com/products/815)和 Raspi。

#### 12 位数模转换器

由于只有一个 PWM 引脚，没有模拟输出，有人将 [Adafruit 12 位 DAC 连接到 Raspberry Pi](http://learn.adafruit.com/mcp4725-12-bit-dac-with-raspberry-pi/overview) 只是时间问题。

#### 16×2 液晶显示器

伺服和 DAC 构建都使用了 [Adafruit I2C 库](https://github.com/adafruit/Adafruit-Raspberry-Pi-Python-Code)和一点 Python。当然，可以将 Raspberry Pi 上的 GPIO 引脚视为数字输出，就像[Mikey]在他的 [Raspi LCD 显示教程](http://learn.adafruit.com/drive-a-16x2-lcd-directly-with-a-raspberry-pi)中所做的那样。

#### 那么，你用的是什么发行版？

当然，所有这些构建都使用了 Adafruit 的 Occidentalis 发行版，这是一个我们之前发布过的对开发者友好的 Linux 发行版。它太有用了，不能作为一个单独的黑客帖子，所以它又来了。