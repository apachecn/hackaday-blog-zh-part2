# 在 GCC 中构建 STM32F0-Discovery 项目的模板

> 原文：<https://hackaday.com/2012/06/17/template-for-building-stm32f0-discovery-project-in-gcc/>

![](img/99299b5444f3c82d748d0da0a6ee1573.png "IMG_20120616_154243")

是的，那个蓝色的灯在闪，是我让它发生的。自从我收到免费的 STM32F0-Discovery 板后，我一直在努力工作。最近，我整理了一个在 Linux 上构建 STM32F05x 项目的模板。您仍然需要安装自己的工具链(我使用的是 Code Sourcery G++: Lite Edition)，但这使得编译支持 STM 外围库的项目变得轻而易举。

至于编程，你可能还记得[我在 stlink 项目](http://hackaday.com/2012/06/04/new-stm32-discovery-board-can-now-be-programmed-on-linux/)中添加了对写入 RAM 的支持。我已经~~浪费了~~大量的时间试图获得对编写 Flash 进入那个项目的支持。使用 stlink 比使用 OpenOCD 要简单得多。但是我真的碰到了一个让 flash loader 代码工作的障碍。如果你想看看我到目前为止在那个领域做了什么，我提交了[一个非常混乱的分支](https://github.com/szczys/stlink/tree/f0-flash-loader-testing)(见[提交](https://github.com/szczys/stlink/commit/1a04fe70ebfcfefd61284d2ab39699b424cb021e)我做了什么代码更改)。

同时，您可以使用 OpenOCD 将使用模板编译的图像写入您的设备。我在 Makefile 中包含了“make program”选项，以便从命令行执行此操作。如果您需要编译 OpenOCD 的帮助，请查看模板库中的自述文件。