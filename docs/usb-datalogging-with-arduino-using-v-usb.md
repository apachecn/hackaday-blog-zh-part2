# 使用 V-USB 通过 Arduino 进行 USB 数据记录

> 原文：<https://hackaday.com/2014/01/18/usb-datalogging-with-arduino-using-v-usb/>

将 USB 功能添加到 Arduino 项目曾经是一件痛苦的事情，但谢天谢地，V-USB 项目的出现让 ATMEGA328 能够直接控制 USB 线路，并模仿简单的(低速)USB 外设。[Ray]通过将 [Arduino 的 I/O 引脚的状态记录到打开的 Excel 电子表格](http://www.hackster.io/rayburne/arduino-to-excel-using-v-usb)中，展示了 V-USB 项目的实现

V-USB ( [虚拟 USB](http://www.obdev.at/products/vusb/index.html) )对于我们这些用 ATMEGA328 构建[独立 Arduino](http://hackaday.com/2010/02/10/the-day-after-arduino/) 项目的人来说尤其有用。与 Arduino Leonardo 及其 ATMEGA32U4 不同，ATMEGA328 没有内置 USB 控制器。连接 USB 线路所需的电路仅由几个基本元件组成，而[Ray]提供了一个参考原理图和 BOM 来帮助您入门。Arduino 被编程为模拟键盘，因此通过允许 Arduino 将数据“键入”到打开的 Excel 电子表格中来实现数据记录。本例中，记录了 8 个数字引脚和所有 6 个模拟输入引脚的状态。

对于那些喜欢 PIC 微控制器并且没有内置 USB 控制器的人来说，有一个 [16FUSB 项目](http://hackaday.com/2012/05/07/16fusb-its-like-v-usb-for-the-pic-16f628/)可以帮助你。