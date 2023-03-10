# 基于 MSP430 的自动喂鱼机

> 原文：<https://hackaday.com/2014/12/08/an-msp430-based-automatic-fish-feeder/>

[Dmitri]想为他的水族馆购买一套自动喂食装置，但是他发现大多数现成的喂食器在份量控制方面都不准确。[Dmitri]的鱼对过度喂食很敏感，所以现成的喂食器无法完成这项工作。由于[Dmitri]对电子学略知一二，他开始着手[建造自己的基于微控制器的自动喂食机](http://www.hackster.io/user3905/fishy-machine)。

[Dmitri]的机器基于一个 MSP430，它在预定的时间开始喂食，并控制分发多少食物。MSP 位于[Dmitri]设计的定制 PCB 上，其中包括步进电机驱动器和终点挡板传感器的输入。该板与步进电机相连，步进电机推动一个上面有一系列孔的小木板。每个洞都装满了一份食物。木板沿着一条 U 形通道滑动，当洞到达通道的末端时，食物从每个洞掉出来，进入水族馆。

整个建筑都有很好的文档记录，[Dmitri]详细解释了他的原理图的每个模块。他的固件也是开源的，所以你可以基于他的设计建造你自己的喂鱼器。休息后，请观看视频，了解喂食器的运行情况。

[https://www.youtube.com/embed/LdPgO7BgAVM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&start=21&wmode=transparent](https://www.youtube.com/embed/LdPgO7BgAVM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&start=21&wmode=transparent)