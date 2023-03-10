# 恒阻假负载设计

> 原文：<https://hackaday.com/2013/02/08/a-constant-resistance-dummy-load-design/>

![constant-resistance-dummy-load](img/aaeec9f2587a07844da4c85f62fa15c9.png)

这个[恒阻假负载](http://embedderslife.wordpress.com/2013/02/07/dummy-load-now-truly-resistive/)还没有经过真实世界的测试。在阅读了[周三的 Re:load 虚拟负载帖子](http://hackaday.com/2013/02/06/reload-an-open-source-dummy-load/)后，【YS】受到了启发，想出了这个电路。那是恒流负载，不是恒阻负载。[YS]从重装的示意图开始，并做了一些改动。

对他来说，这个练习只是改变设计以获得持续的阻力。他实际上并没有构建和测试硬件，因为他并不真正需要它。该图像是从 Proteus 导出的，其中包括一个 ProSPICE 电路仿真器。他的载玻片通过 5V 到 50V 的测试电压，保持恒定的 10 欧姆电阻。

在研究这个项目时，我们需要复习一下不同种类的假负载。[我们发现这篇帖子非常有用](http://electronics.stackexchange.com/questions/38856/constant-current-constant-power-and-constant-impedance-loads/38862#38862)关于恒流、恒功率和恒电阻(阻抗)负载的区别和用途。