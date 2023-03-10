# 使用 AT 命令修改 HC-05 蓝牙模块默认值

> 原文：<https://hackaday.com/2013/09/04/modifying-the-hc-05-bluetooth-module-defaults-using-at-commands/>

HC-05 是一种蓝牙串行桥，在网上售价约为 5 美元，因此可能是为您的项目添加蓝牙连接的最便宜的方式。

但是，它的默认设置可能需要根据您的应用程序进行更改。[Hazim]解释了在命令模式下进入 HC-05[的方法，以便从该设备提供的丰富功能中获益。该过程相当简单，因为它只包括在通电时保持 HC-05 的关键引脚为高电平。然后，设备以默认的 38400 位/秒速度启动命令模式，并监听命令集](http://www.instructables.com/id/Modify-The-HC-05-Bluetooth-Module-Defaults-Using-A/)中的所有[(PDF)。例如，[Hazim]提供了一个草图，允许您直接在自己喜欢的终端上编写 AT 命令。](http://elecfreaks.com/store/download/datasheet/Bluetooth/HC-0305%20serail%20module%20AT%20commamd%20set%20201104%20revised.pdf)

有了基础知识之后，你可能想进一步研究硬件，特别是如果你将使用来自不同来源的模块。它们并不总是带有相同的固件。