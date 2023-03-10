# ATtiny85 草图闪光装置

> 原文：<https://hackaday.com/2012/05/31/attiny85-sketch-flashing-rig/>

![](img/0463034d588da7b5d5babcc8e392e2e9.png "attiny85-sketch-flashing-rig")

我们很高兴看到 Arduino 爱好者在完全不需要基于 ATmega 的主板时支持使用更小的硬件。[Chris]一直在这样做，在他的项目中使用 ATtiny85 芯片。但他厌倦了用跳线来闪现草图。他终于开始着手蚀刻这个 85 编程适配器。

如果项目不需要引脚，[at tiny 85 可以运行 Arduino 草图](http://hackaday.com/2011/09/13/attiny-hacks-run-your-arduino-project-on-an-attiny/)而不需要移植代码。最好的消息是，您用于项目原型的 Arduino 板可以用作独立芯片的编程器。这是一个电路板，克里斯为快速插入设计了双排母插头。在右侧，您可以看到目标芯片的 DIP 插座。虽然这样做效果很好，但我们希望还能包含一个 2×3 AVR ISP 编程头，可用于所有 AT 芯片。