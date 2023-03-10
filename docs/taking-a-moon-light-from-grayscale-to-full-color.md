# 将月光从灰度变为全色

> 原文：<https://hackaday.com/2012/07/06/taking-a-moon-light-from-grayscale-to-full-color/>

![](img/2d12bdf9cbf6c4d102dbc8b5fd045045.png "moon-light-redux")

[特里·米勒]买了一盏便宜的月光灯。它所做的只是通过 LDR 感知夜幕降临后，点亮一些白色 led 来模拟月相。他认为自己可以做得更好，并着手用更丰富多彩的产品取代电子产品。

他选择使用 ATmega328，因为他手头已经有了。该芯片以多路复用方式驱动一系列 RGB LEDs。为了保护 I/O 引脚(并以目标电流驱动 led)，他使用了一组高端和低端 MOSFETs。他决定增加一个红外线接收器，而不是依靠光传感器来打开灯。在休息后的视频中，你可以看到，除了用遥控器开关灯之外，这还让他可以在颜色和效果之间循环。

由于设计中包含的串行接口，当外壳重新组装后，他仍然能够对芯片进行重新编程。该设备由电池供电，其寿命估计包含在他的报告中。

[https://www.youtube.com/embed/dwdsPeqRyNU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/dwdsPeqRyNU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)