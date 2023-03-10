# 使用 Arduino 的简单可编程电子负载

> 原文：<https://hackaday.com/2014/04/29/a-simple-programmable-electronic-load-using-the-arduino/>

有些项目既有教育意义又很有用。我们相信基于 Arduino 的电子负载就是其中之一。

[Jasper 的]电子负载不仅可以作为恒流负载，也可以作为恒功率和恒阻负载。这款多功能器件的设计电压最高可达 30V、5A 和 15W。它基于一个由连接到 Arduino 的 DAC 控制的恒流源。通过测量负载的最终电压和电流，系统可以动态适应以实现稳定性。虽然我们之前已经见过[其他基于 Arduino 的恒定负载](http://hackaday.com/2014/02/24/an-arduino-programmable-load/)，但是相比之下【Jasper 的】非常简单和直接。[Jasper]还包括原理图和 Arduino 代码，这使得它非常容易复制。

电压控制的电流源有很多用途，这个项目是开始建造一个的好方法。这是一个特别好的项目，可以将你的 MOSFET 理论和运算放大器理论知识结合起来！