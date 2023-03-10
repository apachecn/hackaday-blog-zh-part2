# 来自剧院的节日欢呼

> 原文：<https://hackaday.com/2015/01/02/holiday-cheer-from-the-attiny13/>

有比 ATtiny13 更小的微控制器。一些 ARM 芯片将适合一个大引脚的头部，即使在 Atmel world 中，ATtiny10 也采用微小的 SOT-23-6 封装，这种尺寸通常是为表面贴装晶体管保留的。不过，tiny13 几乎可以通过任何 ISP 进行编程，并且采用 8 引脚 DIP 封装。如果你想脱离 Arduino 的世界，这是最起码的，你可以用它做一些非常酷的事情，比如用 SPI 闪存芯片播放一些节日音频。

[Vinod]试图打开一个便宜的相机笔，但在拆卸的过程中，一些痕迹破裂了。他现在只剩下一个 4mb 的 SPI 闪存芯片。这显然是研究用一个小的微控制器和大量的闪存可以做什么的时候了。于是 Attiny13 音频播放器诞生了。

该电路使用一个 PWM 进行音频输出，并直接从闪存芯片读取音频。tiny13 上的 UART 用于更新闪存，还有一个在播放和录制之间选择的开关。如果你正在计算，这意味着有 4 个引脚用于 Flash，2 个引脚用于 UART，1 个引脚用于开关，1 个引脚用于音频输出，以及电源和接地轨，所有这些都在一个 8 引脚封装中。用一个引脚实现两种不同的功能，这是一种非常酷的方式。

你可以看看下面这个项目的视频。

[https://www.youtube.com/embed/c1vg9J15ASs?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/c1vg9J15ASs?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)