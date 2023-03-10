# 3D 打印机的闭环控制

> 原文：<https://hackaday.com/2015/01/20/closed-loop-control-for-3d-printers/>

任何 CNC 机器或 3D 打印机的一个更大的问题是移动工具架时遗漏的步骤。如果步进电机错过了一个步骤，整个印刷层——以及其后的每一层——都会偏离一点点。再错过几个步骤，那张照片最终会被扔进垃圾箱。[Misan]对此有解决方案:[DC 马达的闭环控制](https://www.youmagine.com/designs/dc-motor-closed-loop-control-software#!design-information)用于 3D 打印机。

大多数打印机固件使用开环控制系统来移动它们的马达。朝一个方向走几次，你就知道 3D 打印机的喷嘴会在哪里了。遗漏的步骤混淆了问题，固件没有办法知道喷嘴在任何时候是否在它应该在的地方。

[Misan]对此的解决方案是将 DC 马达与光学编码器耦合。电机和编码器都连接到 Arduino Pro Mini，它接收来自打印机控制器的步进和方向命令。控制器负责告诉电机去哪里，Arduino 负责确保它到达那里。

整个构建在很大程度上来自于[伺服带](https://github.com/danithebest91/ServoStrap)，但是【Misan】有一个非常酷的硬件演示:在打印过程中，他可以将 X 轴和 Y 轴推到任意一侧，每个电机中的 Arduino 会将打印头移回到它需要的位置。你可以看看下面。

[https://www.youtube.com/embed/L-_5KsAOVko?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/L-_5KsAOVko?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)