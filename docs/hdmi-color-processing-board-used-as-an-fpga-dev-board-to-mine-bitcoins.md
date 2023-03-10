# HDMI 彩色处理板用作 FPGA 开发板来挖掘比特币

> 原文：<https://hackaday.com/2013/05/08/hdmi-color-processing-board-used-as-an-fpga-dev-board-to-mine-bitcoins/>

![fpga-eeColor-bitcoin-mining](img/527e8309f7d87075b62440cc4b6a6047.png)

上面看到的蓝色板子是一种叫做 eeColor Color3 的产品的内部结构。它旨在充当电视机和 HDMI 信号源设备之间的通道。它拥有调整色彩饱和度以适应任何观看条件的能力。但是[Taylor Killian]可能不太关心这东西是做什么用的，他把它拆开了，把里面的 FPGA 用于自己的目的。

与合适的开发板相比，这种板的明显问题是引脚没有以用户友好的方式分开。但他在邮件折扣后免费得到了它(如果你幸运的话，你可能会在网上找到一个不到 10 美元的)，它有一个 Altera Cyclone IV 芯片，里面有 30k (EP4CE30F23C6N)栅极，所以他没有抱怨。他的新玩具的第一个项目是加载一个开源的比特币挖掘程序。上图显示，它以每秒 15 兆次的速度运行，而功耗仅为 2.5 瓦。还不错。现在他只需要[做一个模块化的架子](http://hackaday.com/2013/05/07/3d-printer-used-to-make-custom-blade-server-type-mounting-system/)来支撑一个采矿场。