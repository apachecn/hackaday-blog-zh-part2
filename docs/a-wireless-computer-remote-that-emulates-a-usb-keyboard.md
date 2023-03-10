# 模拟 USB 键盘的无线电脑遥控器

> 原文：<https://hackaday.com/2014/05/25/a-wireless-computer-remote-that-emulates-a-usb-keyboard/>

![PCRemote](img/42d0157f97386b5f5cbc700eca8c38d3.png)

如果你有点像[Antoine]，你会喜欢在家里的任何地方用一个简单的手持遥控器控制你的电脑。[Antoine]写信告诉我们他的无线电脑遥控器[模拟 USB 键盘，使其适用于任何使用 USB 键盘的设备。](http://bitsofmymind.com/2014/05/23/the-keymote-a-simple-wireless-remote-for-computers/)

他的博客写得非常好，包含了大量的设计信息和项目背景。他最初想在家里的任何地方轻松控制电脑上的音乐，而不需要在电脑的视线范围内。最终的结果是一个非常方便的遥控器，可以用来改变音乐，视频，甚至在他的电脑上启动应用程序。该系统由连接到计算机并充当 USB 键盘的遥控器基站和遥控器本身组成。基站使用 Arduino 上的 [V-USB](http://www.obdev.at/products/vusb/index.html) 与计算机接口，使用 [VirtualWire](http://www.airspayce.com/mikem/arduino/VirtualWire/) 处理遥控器的无线协议。对于那些不了解 VirtualWire(现已被 [RadioHead](http://www.airspayce.com/mikem/arduino/RadioHead/) 取代)的人来说，这是一个非常酷的 Arduino 库，可以让你轻松使用原始无线接口(也称为[普通无线接口](https://www.sparkfun.com/products/10533))。

无需在此赘述(请务必查看实际帖子以了解更多信息)，遥控器本身在最初的概念验证后进行了重新设计，以最大限度地延长电池寿命。最终功耗非常可观，续航两年以上！这个远程系统被很好地组合在一起，包含了许多方面，可以很容易地被其他项目重用。