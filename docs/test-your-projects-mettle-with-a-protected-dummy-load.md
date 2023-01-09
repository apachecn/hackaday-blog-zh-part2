# 用受保护的模拟负载测试你的项目的勇气

> 原文：<https://hackaday.com/2012/10/01/test-your-projects-mettle-with-a-protected-dummy-load/>

![](img/0469b256dbe8f6b52a65714beae5f85e.png "benchtop")

对于一个耗电量大的项目来说，电力供应有时是一个相当大的未知数。无论是将几个不同的电源钉在一起以满足当前的需求，还是从头开始设计一个系统:一个大电源可能是相当危险的事情。在信任电源来运行你的东西之前，有某种虚拟负载来真正摇下电子设备并了解事物如何变热或测试稳定性是有帮助的。[保罗·奥利维拉]已经建造了这样一个东西，一个光滑的看起来可调的恒流负载。

继流行的 [LM324 电路](http://hackaday.com/2010/08/06/dummy-loads-and-heat-sinks/)之后，来自【大卫·琼斯】的 eev blog【Paulo】决定利用两个备用运算放大器来提供热过载和冷却风扇电路。我们已经看到[过去对【大卫】电路的其他调整](http://hackaday.com/2012/05/15/constant-current-dummy-load/)，但是通过一些电阻和 MOSFETs【保罗】现在可以负载高达 7A(受电阻瓦数限制)。我们会使用一个真正疯狂的服务器~~真空~~风扇，使其真正令人恐惧地推动更重的负载。谢谢[保罗]！