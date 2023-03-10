# 佐克杜伊诺

> 原文：<https://hackaday.com/2014/04/30/the-zorkduino/>

![zork](img/bfce14e4d3889d530290a068964abf64.png)

著名的 Infocom 基于文本的冒险游戏 Zork 实际上是软件工程的技术成就。这是一个令人惊讶的大世界，尽管只是文本形式，运行在一个允许分页、加载和保存完整状态的解释器上。所有这些都是在 70 年代后期为运行在内存不足的计算机上而建造的。你可能认为在 Arduino 上玩 Zork 很容易，但是[rossum]发现，[说起来容易做起来难](http://hackaday.io/project/977-Zorkduino) ( [备用博客链接](http://rossumblog.com/2014/04/29/zorkduino/))

虽然大多数能够运行 Zork 的计算机至少有 8k 的 RAM，但 Arduino 中的 ATMega328 只有 2k 的 RAM。过去那些花哨的家用电脑也有内置视频、键盘，大多数时候还有磁盘驱动器。Arduino 没有这些。

[Rossum]利用 Arduino 的板载硬件直面这一挑战。视频通过 UART 上的 SPI 模式以最高速度–8 MHz 产生。这只是从 SD 卡上的视频缓冲区移出像素。该键盘的处理方式与 Arduino 上的任何其他 PS/2 键盘项目类似，音频是通过以 1000Hz 的频率切换一个按键和 3600Hz 的频率切换 SD 卡访问来生成的。

最终产品包括 SD 卡上的一堆其他 Infocom 游戏，包括*火卫一的皮革女神*，以及可以运行*银河系漫游指南* *，*这个被很多人认为比书更好的游戏。下面视频。

[https://www.youtube.com/embed/-4dWXJrqxUk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/-4dWXJrqxUk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)