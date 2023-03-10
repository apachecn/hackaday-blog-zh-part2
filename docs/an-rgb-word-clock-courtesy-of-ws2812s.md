# 由 WS2812s 提供的 RGB 字时钟

> 原文：<https://hackaday.com/2015/04/12/an-rgb-word-clock-courtesy-of-ws2812s/>

单词钟——用发光的字母而不是数字来显示时间的钟——已经成为标准的 DIY 电子产品；如果你有一个烙铁，这正是你应该建立的。对于[Chris]的字钟构建，[他决定构建一个 RGB 字钟](http://chrisc.bedroomcoders.co.uk/wordclock-build/)。

自从几年前的大海啸以来，发生了很多变化。当时，我们没有很多 ARM 开发板，每个人的祖母都没有使用 WS2812 RGB LED 灯条来超越太阳。[Chris]正在充分利用他所能获得的一切，并使用一个 Teensy 3.1、令人难以置信的[octows 2812 库](https://www.pjrc.com/teensy/td_libs_OctoWS2811.html)和 DMA 来驱动几十个隐藏在激光切割文字模板后面的 led。

结果令人眼花缭乱，但电路很简单——只需一个电平转换器和一个足够大的电源来驱动 led。建筑的机械部分有点棘手，光不可避免地会从外壳中泄漏出来，几张纸刚好能漫射光。尽管如此，这仍然是一个伟大的项目，也是重温经典项目的好方法。