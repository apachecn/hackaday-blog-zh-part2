# 家庭自动化黑客根据人数控制灯光

> 原文：<https://hackaday.com/2012/09/19/home-automation-hack-controls-lights-based-on-head-count/>

![](img/8d208abcb92aa1f83768381711437afd.png "room-occupancy-counter")

这个家庭自动化硬件[根据房间占用率](http://www.instructables.com/id/Room-Visitor-Counter-with-Relay-Control/)打开和关闭灯。该黑客是早期版本的[的扩展，该版本只是概念验证。[RPisces]将这个想法付诸实施，在门口安装了传感器硬件。](http://hackaday.com/2012/07/25/lighting-controller-counts-how-many-people-are-in-a-room/)

他使用 MSP430 launchpad 制作了该设备的原型。它监控一对红外距离传感器，当有东西在它们和走廊对面之间通过时，传感器会记录变化。这是一个很好的传感器选择，因为它只需要通道一侧的硬件。因为使用了其中两个，所以很容易根据哪个先被绊倒来判断一个人是进入还是离开房间。

在这种情况下，[RPisces]驱动继电器打开和关闭灯。但是它可以用于任何事情。我们很乐意看到它触发一个音频系统，就像[Quinn 的]安装在每个房间的那个。