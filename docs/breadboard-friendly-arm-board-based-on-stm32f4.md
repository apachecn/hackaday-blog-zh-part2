# 基于 STM32F4 的实验板友好 ARM 板

> 原文：<https://hackaday.com/2013/11/28/breadboard-friendly-arm-board-based-on-stm32f4/>

![breadboard-friendly-stm32-dev-board](img/5d3c8435478e9a7efeb0db7ba95311a9.png)

嗯，是的……这才像话。STM32F4Stamp 是[Frank Zhao]设计的一个项目，目的是让他的 ARM 原型制作过程更像是过去的 DIP 格式。正如你所看到的，它的宽度仅够在试验板上留出一行跳线。

不要误解我们，[我们真的很喜欢 STM 自己的发现板](http://hackaday.com/2012/11/15/in-depth-comparison-at-stm32-f3-and-f4-discovery-boards/)，因为它们以非常低的价格提供硬件。但是，较大版本(除 F0 变体之外的所有版本)上的双排引脚接头使得连接外围设备变得棘手。这被推到了一个地步，我们看到的发现板的大部分[黑客实际上只是为了](http://hackaday.com/2013/08/07/taming-stm32-discovery-boards-for-regular-use/)[使连接外部硬件更容易](http://hackaday.com/2013/02/15/udp-between-stm32-f4-discovery-boards/)。

你可能会认为这个板缺少了很多东西，但我们不同意。显然，仍然有一个 USB 端口可用于通过 3.3V 调节器为电路板供电。但是，由于 STM32 芯片有内置的引导程序，USB 连接也可以用于将固件刷新到处理器。不错！如果你想自己卷，它是开放的硬件。为了您的方便，我们在休息后嵌入了原理图，以及[Frank 的]演示视频。

[https://www.youtube.com/embed/dJDpkEFYyiw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/dJDpkEFYyiw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[![stm32f4stamp-schematic](img/8f109b040348a20bd701f2a6eb8ac6d4.png)](http://hackaday.com/2013/11/28/breadboard-friendly-arm-board-based-on-stm32f4/stm32f4stamp-schematic/) 【途经[危险原型](http://dangerousprototypes.com/2013/11/20/stm32f4stamp-a-breakout-board-for-stm32f4/)