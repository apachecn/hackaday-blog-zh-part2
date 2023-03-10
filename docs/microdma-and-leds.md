# microdia 和 led

> 原文：<https://hackaday.com/2014/12/04/microdma-and-leds/>

[Jordan]一直在用 TI 的 Tiva 和 Stellaris Launchpads 摆弄 WS2812b RGB LED 灯条。他一直使用 SPI 线路将数据驱动到 LED 灯带，但这种方法意味着处理器需要花费大量时间从存储器位置抓取数据，并将其从 SPI 输出寄存器中取出。这是一个很好的机会来了解这些芯片上可用的μDMA，并编写一个库，使用 DMA 来控制大量的 led，而 SPI 外设无法用简单的代码来处理。

DMA 是一种功能强大的工具，DMA 控制器不会浪费处理器周期在内存和外设之间来回移动位，而是独自做同样的事情，释放 CPU 来做真正的工作。TI 的 Tiva C 系列和 Stellaris LaunchPads 有一个带 32 个通道的μDMA 控制器，每个通道都有四个独特的硬件外设，可以与之交互或用于 DMA 传输。

[Jordan] [编写了一个简单的库](https://github.com/njneerW/WS2812_drv),可以利用 SPI 外设控制一系列 WS2812b LEDs。这比用 CPU 向 SPI 外设传输位要快得多，更新 LED 灯条的帧也更容易；led 动画的新帧可以从主循环中调用，或者 DMA 可以再次启动，而不会浪费宝贵的 CPU 周期来更新一些 LED。