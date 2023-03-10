# 本周失败:EPROM 读取和擦除

> 原文：<https://hackaday.com/2013/10/03/fail-of-the-week-eprom-reading-and-erasing/>

这可能是一个失败，但它确实看起来很酷。[斯科特·劳伦斯]手头上有相当数量的 EPROM 芯片，他决定摆脱传统的橡皮擦和程序员，以便使用自己的硬件来玩概念游戏。他在这个过程的几个步骤中遇到了失望。不过不用担心，每一次挫折都让他重新开始，他学到的东西比实际可行时要多得多。可以说这次失败是非常成功的。

你会想看看围绕这个硬件的两个帖子。最初的想法来自于透过 EPROM 芯片顶部的透明晶体。对[Scott]来说，里面的芯片看起来像一个网球场，他开始想知道当它们被紫外线重新设置时，它们自己看起来是什么样子。他构思了一个 Arduino 附加板，可以读取和擦除芯片。这种设计的 I/O 需求促使他实际制作了一个子板，用于 Arduino 的 MUX shield。这是第一次失败，因为防护罩的工作方式不符合项目的需要。重新设计也让他挠头，但最终他决定使用一些移位寄存器来扩展他的引脚数。

带着这个设计理念，他勇往直前，[建造了 Arduino 盾牌(见上图](http://geodesicsphere.blogspot.com/2012/11/eproms-part-2-success.html))。这些零件号不是你所期望的移位寄存器。他最终走了一条有点不同的路线，从一个旧的 Amiga 附加板上回收了这些 74LS393 芯片。这非常有效。用于擦除芯片的双紫外发光二极管一点也不起作用。他将被擦除的位可视化的梦想已经破灭，但他确实看到了光明的一面，他现在有办法使用 Arduino 读取 EPROM。

* * *

**[![2013-09-05-Hackaday-Fail-tips-tile](img/4ddcb45ba24697ecb36e5a2da073e8dc.png)](mailto:tips@hackaday.com?Subject=[Fail of the Week]) 每周失败是一个每周三运行的黑客专栏。通过写下你过去的失败和[给我们发送一个故事的链接](mailto:tips@hackaday.com?Subject=[Fail of the Week])，或者发送你在互联网旅行中发现的失败报道的链接，来帮助保持乐趣。**