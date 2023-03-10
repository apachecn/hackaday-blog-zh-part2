# CPLD 教程:轻松学习可编程逻辑

> 原文：<https://hackaday.com/2014/04/06/cpld-tutorial-learn-programmable-logic-the-easy-way/>

hackshed 那边的人很忙。[Carl]正在用 8 部分 CPLD 教程使可编程逻辑设计变得简单。(2018 年 3 月:链接死。试试[返程机](https://web.archive.org/web/20170629090531/http://www.hackshed.co.uk/getting-started-with-cplds-index/)。)可编程逻辑器件是黑客可用的最通用的硬件构建模块之一。他们也可以有一个陡峭的学习曲线。廉价的[现场可编程门阵列](https://en.wikipedia.org/wiki/Fpga) (FPGA)比比皆是，但可能有复杂的功率要求。大多数现代可编程逻辑设计都是用硬件描述语言(HDL)创建的，如 VHDL 或 Verilog。现在你有了一种新的设备，一种新的语言，一个全新的编程范例，以及一个复杂的 IDE 来一次性学习。难怪 FPGAs 会让不止一个初学者退避三舍。

本教程从几个方面缩短了学习曲线。【卡尔】正在使用[复杂可编程逻辑器件](https://en.wikipedia.org/wiki/CPLD) (CPLD)。在 40，000 英尺的高度，CPLDs 和 FPGAs 做同样的事情——它们充当可重新配置的逻辑。FPGAs 通常不存储其配置，必须从外部闪存、EEPROM 或连接的处理器加载。CPLDs 会存储它们的配置，所以它们一上电就准备好了。一般来说，FPGAs 比 CPLDs 包含更多可配置逻辑。这允许用 FPGAs 实例化更大的设计。但是不要批评 CPLDs。CPLDs 为大设计留有足够的空间，比如产生 VGA 信号的。

[Carl]也在他的教程中设计了示意图捕获。使用原理图捕获方法，可以像在 Eagle 或 KiCad 中一样绘制数字逻辑原理图。这通常被认为是一种“老派”的设计捕捉方法。几行 VHDL 或 Verilog 代码可以代替一些相当复杂的原理图。虽然简单的设计不需要那种力量。走原理图捕获路线消除了学习 VHDL 或 Verilog 的需要。

【卡尔的】教程从安装 Altera 的 Quartus II 软件开始。然后，他带领学生进入“硬件你好世界”LED 闪烁。教程完成时，用户将学习如何创建一个 4 位加法器和一个 4 位减法器。有了这些，你就准备好投入到大的设计中去了——[比如建造一台逆向计算机](http://hackaday.com/2014/02/17/a-pick-and-mix-fpga-retrocomputer/)。

[图片来自[维基共享资源](http://commons.wikimedia.org/wiki/File:Altera_MAX_7128_2500_gate_CPLD.jpg)