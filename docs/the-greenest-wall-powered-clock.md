# 最环保的挂钟

> 原文：<https://hackaday.com/2013/10/13/the-greenest-wall-powered-clock/>

![clock](img/6101309031b64c979ef43db6c9bece85.png)

一些最低效的家用电器是交流电源供电的时钟。你不能完全关掉它们，考虑到它们被注视的频率，它们会消耗大量的能量。[t3andy]想出了一个很棒的[低功率交流电源时钟](http://forum.pjrc.com/threads/24319-NeoPixel-Teensy-3-Green-AC-Mains-Clock-Project-The-greenest-AC-Mains-Clock-in-USA)，它只在 3%的时间里工作。另外，它看起来也非常非常酷。

[t3andy]使用 Teensy 3 作为这个时钟的大脑，板上的串行接口提供了一种相对简单的设置时间的方法，无需使用按钮或轻触开关。钟面由 13 个[新像素](http://www.adafruit.com/products/1260)组成，两个红色像素显示小时，一个绿色像素显示分钟。时间是用带备用电池的 DS3232 I2C 实时时钟测量的。

这种设计非常有效，因为 led 在 97%的时间里都是关闭的，只有在一分钟的顶部才被点亮。有红外控制和 PIR 传感器的规定，以便在需要时显示时间，但这显然意味着对能源效率的打击。