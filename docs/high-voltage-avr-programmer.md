# 高压 AVR 编程器

> 原文：<https://hackaday.com/2015/04/09/high-voltage-avr-programmer/>

AVR 微控制器最常见的编程方式是系统内编程端口。那个带 MOSIs 和 MISOs 的小 6 针接头可以编程你遇到的每一个 AVR。ISP 也有不利的一面——保险丝。设置你的保险丝错误，没有高压串行编程器，你的芯片是砖砌的。[[dil shan]设计了自己的 HVSP](http://hackaday.io/project/5179-avr-hv-high-voltage-programmer-for-avr-mcus)，比 Atmel STK500 便宜，并且有一个很好的 GUI 应用程序。

[Dilshan]没有跟随 USBtinyISP 的脚步，而是使用 PIC18F 作为编程器中的主微控制器。选择这款芯片是因为它内置了 USB 功能。因为 HVSP 的高压部分在 12V 下工作，所以实际提供的电压需要考虑在内。为此，[Dilshan]使用标准 78xx 稳压器，输入电压为 18V。

控制这个程序员的应用程序做了你所期望的一切，包括所有常用的 AVRdude 命令。一个伟大的构建，正是我们所需要的重新设置我们周围几十个芯片上的保险丝。