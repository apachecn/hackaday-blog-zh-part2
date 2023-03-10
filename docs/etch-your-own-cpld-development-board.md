# 蚀刻您自己的 CPLD 开发板

> 原文：<https://hackaday.com/2013/05/28/etch-your-own-cpld-development-board/>

![etch-your-own-cpld-breakout](img/96ecafbb2d9ff34d7ff0b1aa36263102.png)

曾经想从微控制器跳到逻辑芯片吗？虽然从技术上讲不是一回事，但我们认为 FPGA 和 CPLD 器件属于类似的类别。像 FPGAs 一样，复杂的可编程逻辑器件允许你在芯片内部构建硬件。如果你已经掌握了蚀刻电路板的诀窍，你现在可以[建立自己的 CPLD 开发模块](http://startingelectronics.com/projects/xilinx-CPLD-board/)。长期的 Hackaday 读者会记得[我们在这方面的产品](http://hackaday.com/2008/12/11/how-to-programmable-logic-devices-cpld/)。

我们多年的微控制器经验教会了我们一句口头禅:如果它不起作用，那就是硬件问题。我们有浪费时间试图找出为什么我们的代码不工作的诀窍。大多数情况下是硬件问题。这就是为什么你可能不想在刚开始的时候设计自己的开发工具。但是这个指南有一个优点就是增量测试。蚀刻和检查电路板后，分阶段组装。每个阶段都有测试代码，有助于验证硬件是否按预期工作。

CPLD 使用该 10 引脚接头进行编程。如果你没有程序员，你可以[使用并行端口](http://startingelectronics.com/projects/xilinx-parallel-programmer/)构建自己的程序。板上包括一个 ATtiny2313，这是一个很好的接触，因为它可以模拟各种不同的硬件来测试你的 VHDL 代码。还有一排 led、一组 DIP 开关和几个分接头。