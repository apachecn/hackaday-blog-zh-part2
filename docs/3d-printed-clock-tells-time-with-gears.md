# 3D 打印时钟通过齿轮显示时间

> 原文：<https://hackaday.com/2014/12/01/3d-printed-clock-tells-time-with-gears/>

[ekaggrat]设计了一个 [3d 打印时钟](https://hackaday.io/project/3499-holo-clock)，制作相当简单，看起来棒极了。这种时钟有一系列 3d 打印的齿轮，都是由一个步进电机驱动的，[ekaggrat]发现过剩。

时钟的控制器基于用 Arduino IDE 编程的 ATtiny2313。ATtiny 控制用于运行步进电机的达林顿驱动器 IC。ATtiny 每分钟向前驱动步进电机，通过 3d 打印的齿轮移动时针和分针。小时和分钟由大齿轮内的两个橙色柱指示。

[ekaggrat]为微控制器和步进驱动器蚀刻了他自己的 PCB，使得构造美观紧凑。如果你想建造你自己的，[ekaggrat]在 GitHub 上发布了他所有的设计文件。你所需要的只是一块印刷电路板(或试验板)、一些元件和一台 3D 打印机上的一点时间来制作你自己的时钟。