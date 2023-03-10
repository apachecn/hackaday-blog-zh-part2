# 对 HP-IB 磁盘驱动器进行成像和仿真

> 原文：<https://hackaday.com/2015/06/20/imaging-and-emulating-an-hp-ib-disk-drive/>

如果你看看旧的测试设备的背面，你会发现一个奇怪的连接器，要么标着 IEEE-488，GPIB，要么标着 HP-IB。这是一个由惠普为他们的测试设备设计的非常旧的接口，它被授权给其他制造商用于从电源到逻辑分析仪的一切。惠普从前也做过电脑和工作站，这种接口也进了这些盒子也就不足为奇了。他们甚至有通过 HP-IB 接口操作的外部硬盘。

[Chris]有几台这样的旧电脑，[想看看他是否能模仿这些 HP-IB 硬盘中的](http://www.insentricity.com/a.cl/242/emulating-an-old-hp-ib-disk-drive-with-hpdrive)。[有一个项目是仿真这些硬盘](http://www.hp9845.net/9845/projects/hpdrive/)，但是电气连接有点棘手；你需要一个 IEEE-488 卡，这些卡已经不再生产了。

然而，[克里斯]去年找到了一个旧的 ISA IEEE-488，并将其安装在他用于所有复古探索的 PC 系统中。在将卡和电缆安装到他的 PC 上后，[Chris]将一个真正的 HP-IB 磁盘连接到他运行 HPDrive 的现代计算机上，制作了一个映像，并连接了一台旧的 HP 150 计算机。图像由 HP 150 读取，而[Chris]有一台老式计算机运行模拟驱动器。