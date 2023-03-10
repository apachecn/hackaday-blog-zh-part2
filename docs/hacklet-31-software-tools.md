# hacklet 31–软件工具

> 原文：<https://hackaday.com/2015/01/23/hacklet-31-software-tools/>

对于每一个计算机错误，都有两个人为错误，其中之一是责怪计算机。每当人类因为某件事责备计算机时，有两种工具，其中之一就是计算机。

不是所有你的漂亮工具都需要是花哨的机器人、数控机床或漂亮的罗伯逊螺丝刀；只要有合适的软件，电脑同样可以成为一个神奇的工具。在本周的 Hacklet 中，我们将浏览 [hackaday.io](http://hackaday.io/) 上一些最好的*软件*工具。

![6653681421957570397](img/cf0cec8043899381cebdcec875c8db5a.png)【艾伦】受到启发，打造了[一款制作缝纫图案的软件工具](http://hackaday.io/project/4033-digital-patterns-for-sewing)。缝纫图案通常是为“普通”人设计的，但如果你正在制作定制的可穿戴设备，你最终应该得到一件完全合身的衣服。

第一个项目[艾伦]使用这个工具是一个羊毛帽，适合他的头部轮廓。他捕获了他头部的 3D 网格，将网格导入到 Blender 中，并打开生成的网格。帽子的两半用羊毛剪出轮廓浮雕，然后缝合在一起。结果是一顶帽子完美地套在了艾伦的头上。这是一个非常酷和新颖的 3D 建模应用，如果你需要用 2D 材料包裹 3D 物体，这就是你想要的项目。

你认为 Eagle 的自动路由器不好。

[Anderson]开发了一个叫做黄铁矿的工具，它可以获取一个示意图，并在三维空间中构建一个布局。他称之为[体积电路](http://hackaday.io/project/2396-volumetric-circuits)，它基本上是老式收音机和放大器中发现的点对点线路，发展到下一个水平。[我们在](http://hackaday.com/2014/09/13/volumetric-circuits/)之前就推出了这个项目，从那以后就没有太多更新了。也许给[安德森]的项目一些建议会有助于激励他回到项目中来。

![133031421839442989](img/fa1985179129d81813b350faf702900a.png)不满足于现有的免费开源 CAM 程序，[【Snegovick】开始了自己的](http://hackaday.io/project/3985-bcam-2d-computer-aided-manufacturing)工作。

[Snegovick]称他的项目为 BCAM，这正是你需要在 PCB 上磨孔，用 CNC 路由器切割齿轮，雕刻塑料，以及 2.5 轴 CNC 机器可以做的任何事情。项目是用 Python 写的，没错，[源码可用](https://github.com/snegovick/bcam)。支持的操作包括钻孔、路径跟踪、偏移路径跟踪和装袋。

编写足够多的微控制器项目，最终你会有自己的通用代码库，它能做好一件事，又能做好一件事。如果你够聪明，你会在未来的项目中重用这些代码。[ericwazhung] [正在突破开发所有这些代码](http://hackaday.io/project/3828-commoncode-not-exclusively-for-avrs)的困难部分，并发布了一些在许多项目中有用的东西。

commonCode 库中包括常见的“心跳 LED”，非阻塞输入，AVR 定时器的标准接口，文本字符的位图，DC 电机控制，等等。在任何情况下都非常有用。

这就是这一轮 Hacklet 的全部内容，为您带来最好的 [hackaday.io](http://hackaday.io/) 内容。