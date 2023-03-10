# 每秒 5 兆样本的 Arduino 示波器

> 原文：<https://hackaday.com/2013/07/08/arduino-oscilloscope-at-five-megasamples-per-second/>

在你的电子工作台上，没有什么可以替代一个合适的示波器。但不幸的是，我们还没有自己的车。但我们有一个 Arduino 板，并与另一个 IC 配对，它可以[每秒采样惊人的 500 万个周期](http://bobdavis321.blogspot.com/2013/06/arduino-powered-3-million-samples-per.html)。

[鲍伯·戴维斯]已经研究了一段时间基于 Arduino 的 oscillscope。他不断从中挤出越来越多的表演。之前的版本使用 AD775 芯片达到 300 万样本。当他添加一个 FIFO 缓冲芯片时，他能够从中挤出 10-25 兆样本…哇！不幸的是，输出往往是假的。

该版本取消了 AD775，采用了 CA3306。两者都是模数转换器，但新电路更简单、更可靠。它仅使用三个电容和一个外部时钟来支持 IC。看看下面的视频，看看它的表现如何。他正在一个小的液晶显示屏上输出样本的图表。最好的部分是，由于额外的芯片正在进行采样，这可以移植到您选择的微控制器。

[https://www.youtube.com/embed/f_RD1oQuKiw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/f_RD1oQuKiw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)