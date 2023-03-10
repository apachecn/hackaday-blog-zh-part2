# STM32 开发板令人印象深刻

> 原文：<https://hackaday.com/2013/02/19/impressive-dev-boards-for-your-stm32-dev-boards/>

![stm32-discovery-breakout-boards](img/5086f1d6cfb3adada42a32cdd436420a.png)

似乎有很多人对 STM32 发现板有相同的抱怨；很难向它们添加外部硬件。不要误解我们，我们欣赏所有的引脚被打破(相对于 Stellaris Launchpad，我们认为可用的太少)。以下是斯科特·科尔纳克对这个问题的解决方案。他制作了三种不同的基板，STM32 Discovery 可以插入其中。每一款都适用于不同型号的开发板:VL、F3 和 F4。但他也认为[我们在另一个项目](http://hackaday.com/2013/02/15/udp-between-stm32-f4-discovery-boards/)中看到的基板是 F4 解决方案的一个不错的选择。

这些大型 PCB 附件以两种不同的方式提供功能。第一种方法是使用可扩展端口接入串行通信连接器或模拟/SPI/I2C 模块等模块。对我们来说，第二种方法是最可取的。他将每个 GPIO 端口连接到一个 2×8 接头，并使用 IDC 电缆(这些图片中的彩虹电缆)将其连接到试验板。看到这种情况，我们希望 STM 使用 16 针的离散簇，而不是那些超长的双针接头。