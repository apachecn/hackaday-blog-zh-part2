# 用于物理计算的触觉手环

> 原文：<https://hackaday.com/2015/02/12/a-haptic-bracelet-for-physical-computing/>

[Tinkermax]一直在阅读关于物联网和可穿戴计算的资料，并决定是时候让他尝试构建一种将计算变成物理的设备了。结果是一个振动腕带将他的触觉连接到互联网。

这种触觉腕带的电子设备是新旧技术的结合。无线电和微控制器来自 ESP-8266 模块，该模块用[【米哈伊尔·格里戈里耶夫】的非官方 SDK](http://programs74.ru/udkew-en.html) 编程。腕戴式计算机的机械结构由安装在手腕上的六个寻呼机电机组成。这些都是由一个 TLC5917 LED 驱动芯片巧妙地驱动[。这意味着 ESP 只需要使用两个 GPIOs 来控制六个电机。](http://www.ti.com/product/tlc5917)

现在软件足够简单；只有一个网页，几个按钮，并能够通过互联网按动腕带上的任何寻呼机电机。现在的问题只是让这种可穿戴设备变得有用，但将每个寻呼机电机连接到不同的通知——新电子邮件、新短信或互联网上的一些紧急情况——应该很容易。

下面视频。

[https://videopress.com/embed/TIySIoiN?hd=1&cover=1&loop=0&autoPlay=0&permalink=1&muted=0&controls=1&playsinline=0&useAverageColor=0](https://videopress.com/embed/TIySIoiN?hd=1&cover=1&loop=0&autoPlay=0&permalink=1&muted=0&controls=1&playsinline=0&useAverageColor=0)