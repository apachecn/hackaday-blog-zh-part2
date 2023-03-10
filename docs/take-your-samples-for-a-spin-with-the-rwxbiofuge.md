# 用 RWXBioFuge 旋转一下你的样品

> 原文：<https://hackaday.com/2014/10/21/take-your-samples-for-a-spin-with-the-rwxbiofuge/>

我们要坦白:我们热爱离心机。我们已经使用了所有的形状和大小，将全血袋纺成单独的成分来提取 DNA，以及这之间的一切。不幸的是，这些实验室必需品对于许多 DIY 生物学家来说太贵了，除非他们购买二手的或者自己制作。[Pieter van Boheemen]受到其他 DIY 离心机的启发，决定制作自己的离心机，并将其命名为[rwxfiofuge](https://github.com/PieterVanBoheemen/RWXBioFuge)。

[Pieter]使用 Sketchup、OpenSCAD 和 InkScape 设计了 RWXBioFuge。它具有一个 Thermaltake 智能 M850W ATX 电源，一个遥控直升机电子速度控制器(ESC)，和无刷 outrunner 电机。对于用户输出，它利用一个 16×2 液晶字符显示器与 I2C 接口。框架由 3 毫米 MDF 激光切割而成，而 3D 打印的 PLA 转子设计有 [OpenSCAD](http://www.openscad.org/) 。

Arduino 处理事物的处理方面。[Pieter]使用 Arduino 以太网–允许网络界面远程控制离心机的设置和操作。我们可以看到这在测试离心机的任何转子/电机平衡问题时是有用的，特别是因为[Pieter]指出它可以配置为以大于 10，000 rpm 的速度运行。如果碎片以那样的速度从离心机上飞出，我们就不想待在这个房间里了！然而，我们认为，当你在实验室工作时，你应该有一台可以信赖的离心机在你身边。

虽然与 [Openfuge 有相似之处，但](http://hackaday.com/2013/09/23/openfuge-an-open-source-centrifuge/)更大的 RWXBioFuge 具有[八个](http://www.thingiverse.com/thing:97524)到[二十个](https://www.youmagine.com/designs/microcentrifuge-20-place-rotor)1.5-2.0 毫升微量离心管的转子容量。由于电源的原因，它不是便携式的，有点贵，但也不是难以置信的贵。这台离心机有一些我们非常喜欢的小细节。开盖检测机始终是一项受欢迎的安全功能。“短”按钮对于快速旋转 5-10 秒非常方便。

RWXBioFuge 的最新版本正在 Waag 协会的开放湿实验室中使用。【Pieter 的】下一版本的计划升级包括磁性盖锁、不同的转子尺寸、用于检测不平衡转子的加速度计，以及优化电源、ESC 和电机设置。实验室里的离心机永远都不够用，我们期待看到这个项目的进展！

休息之后，再来看看几张 RWXBioFuge 的照片。

![More images of the RWXBioFuge](img/405407adb3c5d117f0122c9e024dae68.png)