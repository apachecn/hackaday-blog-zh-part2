# Raspi 迷你激光雕刻机

> 原文：<https://hackaday.com/2013/11/23/raspi-mini-laser-engraver/>

如果你有很多备用零件，你也许可以毫不费力地拼凑出自己的激光雕刻机。我们已经看到了使用 Arduino 的[小型雕刻师构建，但[Jeremy]向我们透露了[香斋的]版本，它提供了用树莓皮构建一个的深入指导。](http://hackaday.com/2013/10/27/microslice-the-tiny-arduino-laser-cutter/)

[向]首先打开了两个备用的 DVD 可写驱动器，不仅回收了它们的激光二极管，还回收了步进电机及其附带的硬件，以及每个二极管附近的一些小磁铁。为了组装激光器，他从易贝采购了一种廉价的激光二极管模块，并用老虎钳将二极管推入外壳的头部。把雷射放在适当的位置，并焊上适当的连接线，[翔]很快就完成了一个雷射驱动电路，Raspi 稍后会控制这个电路。[向]按照[格罗佛的]雕刻机的构造设计出了步进电机的配置-(我们几年前[介绍过它](http://hackaday.com/2011/03/11/bench-top-laser-engraver-does-some-cutting-too/))-将固定待雕刻材料的板连接到一个轴上，将激光组件连接到另一个轴上。

查看[Xiang]的项目博客，了解解释 h 桥电路以及 Raspi 的 Python 代码的详细信息。和往常一样，如果你尝试任何涉及激光的构建，请使用所有必要的预防措施！如果你需要更多关于使用 DVD 刻录机的信息，请查看这个夏天早些时候的黑客攻击