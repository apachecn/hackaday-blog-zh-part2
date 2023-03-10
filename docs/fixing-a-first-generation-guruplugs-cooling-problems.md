# 修复第一代 GuruPlug 的冷却问题

> 原文：<https://hackaday.com/2012/10/25/fixing-a-first-generation-guruplugs-cooling-problems/>

![](img/8afa8fb6e2f39635fdf2e5a916b01bd5.png "guruplug-cooling-mod")

[Doragasu]一直使用被黑的 Xbox 作为他的文件服务器，但在 GuruPlug 发布时升级到了单板 Linux 设备。不幸的是，这些设备的第一次运行出现了过热问题，导致即使在中等 CPU 负载下也要重新启动。设计从被动冷却散热器改为内部风扇，但这并没有真正帮助那些已经有一个早期型号的人。以上是【剑龙】[冷却过热电脑](http://kernelhacks.blogspot.com/2012/04/my-guruplug-usblcd.html)的方法。

原来的散热器——实际上只是一个无鳍的金属板——被移除并替换为一个合适的散热器。这与 ARM、RAM 和以太网芯片接触。它们在安装前都涂上了热化合物，并增加了一个静音风扇来帮助驱散热量。这仍然适合在原来的情况下，但为了让路，他没有删除原来的电源，并削减了一个洞，让空气流动。

这篇文章还详细介绍了用于显示系统信息的外部液晶屏。这与这个 USB 液晶显示屏项目是一脉相承的，正是这个项目启发他给我们发来了这个项目的链接。