# 来自 MSP430 的 MSP430 闪存仿真工具

> 原文：<https://hackaday.com/2014/10/06/an-msp430-flash-emulation-tool-from-an-msp430/>

对 TI 的 MSP430 芯片进行编程并不困难，但是除了官方的 Flash 仿真工具之外，TI 并没有降低对这些微控制器进行编程的成本。MSP 430 最常见的编程方式是使用 Launchpad 开发板，【文森特】[拥有迄今为止最好看的开发板](http://r6500.blogspot.com.es/2014/10/msp340-launchpad-fet.html)。

MSP430 系列芯片可以通过 JTAG 或线控间谍进行编程，TI 为这些芯片提供的官方专业工程工具[价格约为 100 美元](http://www.ti.com/tool/msp-fet)。我们这些比金钱更明智的人有另一个选择——使用 TI Launchpad 开发板作为 MSP430 程序员。

[Vicente]的项目使用 MSP430G2 Launchpad，只有几根电线连接到 TI 官方编程器中的正确连接器。有一些限制；编程器只能在 3.6V 下工作，因此对 1.8V 器件编程可能不是一个好主意。此外，它只能与线控间谍和没有 JTAG 支持可用。尽管如此，这仍然是一个看起来很棒的项目，并且完全按照它的设计去做。