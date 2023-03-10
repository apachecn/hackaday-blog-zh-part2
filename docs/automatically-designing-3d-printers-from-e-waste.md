# 从电子垃圾中自动设计 3D 打印机

> 原文：<https://hackaday.com/2015/07/20/automatically-designing-3d-printers-from-e-waste/>

没有人想设计寿命超过几年的消费电子产品。这种趋势是一场生态灾难，数百万吨的电脑、打印机、传真机和手机最终被扔进了垃圾填埋场。在这些垃圾填埋场中，所有用于提取微量镀金的铅和化学物质都会渗入环境中。彻底改变它是巨大的，但是再利用一些废物可以有所作为。

[Masterperson]和[Maaphoo]一直在研究如何将成吨的电子垃圾变成有用的东西。他们提出了一个将电子垃圾转化为 3D 打印机的框架。通过 Python 和 FreeCAD 宏的巧妙应用，该项目可以使用从废弃的 2D 打印机中取出的电机、轴和轴承来生成 3D 打印机的模型。

现在，可以通过将手头的部件添加到配置文件中来配置打印机，在 FreeCAD 中运行 Python 宏，等待宏生成部件来构建笛卡尔机器人。该宏还为需要打印的零件提供文件，并可与[制版机](https://github.com/RobotsWar/Plater)接口，以优化这些打印零件在现有打印机上的位置。

这是一个非常酷的项目，但还没有完成:该团队正在寻求帮助来完善打印机设计，并可能开发出比简单的笛卡尔机器人更多的设计。任何明确旨在从 2D 打印机上摘下肉的东西都是一个好主意，而将这些变成真正的 3D 打印机是最重要的。