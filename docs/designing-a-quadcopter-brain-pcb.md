# 设计四轴飞行器大脑 PCB

> 原文：<https://hackaday.com/2012/07/27/designing-a-quadcopter-brain-pcb/>

![](img/629f9fd17e280386a69a25e66a6e5993.png "designing-a-quadcopter-brain-pcb")

在从事他的四轴飞行器项目时，[Matt]决定最好为该设备制造一个鲁棒的控制器。他从未发送过 PCB 设计用于制造，但他大胆尝试，第一次尝试就完成了紧凑可靠的 PCB。

当我们听到四轴飞行器控制器时，首先想到的是反馈传感器。用于这些项目的加速度计通常采用 DFN 或 QFN 封装。这意味着没有腿。相反，芯片在封装底部有焊盘，使得焊接更加困难。[Matt]通过使用已经安装了传感器的 IMU 板回避了这个问题，并提供了一个 0.1”SIL 引脚接头作为接口。这很容易融入设计中，以及所有其他用于电机控制、电源等的连接器。他拿了一份 Eagle Lite 来做布局，并使用 [OSH Park](http://hackaday.com/2012/06/28/an-interview-with-lean-the-force-behind-dorkbot-pdx/) 来制作电路板。他很惊讶第一次尝试就万事大吉了。由于他的计划，它适合放在一个塑料食品容器内，在那里它应该能够轻松地度过大多数轻微的碰撞。