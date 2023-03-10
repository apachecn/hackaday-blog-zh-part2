# 用 LED 灯条建造巨大的显示屏

> 原文：<https://hackaday.com/2013/02/25/building-huge-displays-with-led-strips/>

构建 RGB LED 显示屏是我们在 Hackaday 上看到的最有趣的编程和工程挑战之一。不仅大型显示器和 LED 立方体的创造者必须处理驱动整个 LED 束的功率需求，而且还有获得足够高的帧速率以显示视频的问题。这是一项艰巨的任务，但[保罗·斯托佛雷根]有一个有趣的解决方案。他编写了一个 LED 灯条库，可以控制 8 米长的 LED 灯条，这些灯条也可以用在菊花链 Teensy 3.0 微控制器上，用于非常大的显示器。

[Paul]的 LED 库使用基于 WS2811 LED 控制器 IC 的 LED 灯条。这些芯片是最常见的独立可控 LED 灯条控制器芯片，你可以在 Adafruit 或数百家中国经销商那里找到[。图书馆需要 DMA 传输来显示图像，所以如果你正在寻找建立一个巨大的 RGB LED 显示器，你可能会想拿起几个](http://www.adafruit.com/products/1138)[【保罗】的 Teensy 3.0 板](http://www.pjrc.com/store/teensy3.html)

[Paul]还开发了一个处理应用程序，可以将视频文件转化为串行数据，用于他的 LED 灯带库。休息之后，你可以看看这个应用程序、库和 60×32 RGB LED 显示屏的视频。

[https://www.youtube.com/embed/M5XQLvFPcBM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/M5XQLvFPcBM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)