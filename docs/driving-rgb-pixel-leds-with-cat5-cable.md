# 用 CAT5 电缆驱动 RGB 像素 led

> 原文：<https://hackaday.com/2014/02/09/driving-rgb-pixel-leds-with-cat5-cable/>

![cable-test](img/ceb53e8fb8ce5db57941a7c460593f17.png)

[Teknynja]正在进行一个项目，他需要驱动几条 Adafruit neo pixels(ws 2812 LED 条),它们相距几英尺。这些 LED 灯条消耗大量电流，并且对时间非常敏感；微控制器和 LED 灯条之间的任何超过几英尺的电线都可能导致数据丢失、电压下降、LED 变暗，并可能导致灯条不起作用。

和所有关于远距离数据传输的问题一样，解决方案是 CAT5 电缆。【Teknynja】使用 RS-422 驱动器和接收器来完成这项任务，75174 线路驱动器接收来自 Teensy 3.0 的信号，75176 总线收发器读取 20 英尺电缆另一端的所有数据。

对于功率下降问题，[Teknynja]正在向电缆中的一些线对馈送 12V 电压，并使用廉价的 LM2596 降压转换器将条带处的所有电压降至 5V。

通过一个相当简单的电路，[Teknynja]能够通过 20 英尺长的 CAT5 电缆轻松驱动几条 WS2812 LEDs 它的工作原理就像像素直接连接到工作台上的面板上一样。