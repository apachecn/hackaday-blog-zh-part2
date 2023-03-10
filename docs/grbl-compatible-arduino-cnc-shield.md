# GRBL 兼容 Arduino CNC 屏蔽

> 原文：<https://hackaday.com/2013/07/28/grbl-compatible-arduino-cnc-shield/>

当你在家用 CNC 系统中添加控制电子设备时，你可能已经准备好用最简单的方法达到可能的目的。在这种情况下，拿起你的 Arduino，加热蚀刻溶液[制作你自己的 GRBL 兼容屏蔽](http://blog.protoneer.co.nz/arduino-cnc-shield/)。

这个熟悉的占地面积设法包含三轴机器所需的一切。插入 SIL 接头对的紫色板是 Pololu 步进电机驱动器。走这条路使得更换烧坏的芯片像插上新模块一样容易。中间的端子板为驱动电机所需的高压轨供电。右侧的 DIL 标题断开了与限位开关(每个轴两个)、主轴和冷却剂控制以及暂停、恢复和中止三个按钮的所有连接。甚至还有一个 SPI 头，如果需要，可以更容易地添加定制硬件。

这是一个双层板，可能不适合您自己的制造工艺。[Bert Kruger]发布了他的 Gerber 文件供下载，如果你想在 OSH Park 或类似的服务中运行。