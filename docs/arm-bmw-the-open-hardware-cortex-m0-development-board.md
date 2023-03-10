# ARM-BMW，开放硬件 Cortex-M0 开发板

> 原文：<https://hackaday.com/2014/08/26/arm-bmw-the-open-hardware-cortex-m0-development-board/>

[![](img/b5dd94c6342e7026c793b26cc9c807c7.png)](https://hackaday.com/wp-content/uploads/2014/08/frontq-1500px.jpg)

[Vsergeev]向我们透露了一款基于 Cortex-M0 的开发板，总 BoM 成本不到 15 美元。它被称为 ARM 裸机部件(ARM-BMW)，专注于电池电量、非易失性存储和可调试性。

选择的微控制器是 50MHz [恩智浦 LPC1114DH28](http://www.nxp.com/products/microcontrollers/cortex_m0_m0/lpc1100/LPC1114FDH28.html) ，它为用户提供 32kB 闪存、8kB SRAM、6 通道 ADC 和 I2C/SPI/UART 接口等。ARM-BMW 包含一个 2mb SPI 闪存、一个 I2C I/O 扩展器、几个用于扩展/调试目的的接头、4 个 led、2 个按钮、2 个 DIP 开关以及一个用于闪烁和调试的 JTAG/SWD 接头。如上图所示，您可以安装自己的 HC49UP 晶体或使用内部 12MHz RC 振荡器。

该平台可以使用 USB 电缆或 LiPo 电池供电。正如你所猜测的，它还包括一个急需的电池充电器(MCP73831T)和一个开关电容 DC/DC 转换器，以提供 3.3V 电源。你可能会在[硬件](https://github.com/vsergeev/arm-bmw-hw)或[软件](https://github.com/vsergeev/arm-bmw-sw)存储库中找到所有文件。