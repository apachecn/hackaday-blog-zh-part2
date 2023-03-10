# 作为 PIC 程序员的 Raspberry Pi

> 原文：<https://hackaday.com/2012/08/17/raspberry-pi-as-a-pic-programmer/>

![](img/a2caa5baa9247dea934f815ff1fde1de.png "rpi-pic-programmer")

[Giorgio Vazzana] [用一个相当小的通用部件集合，把他的树莓 Pi 变成了 PIC 程序员](http://holdenc.altervista.org/rpp/)。它支持 16F 系列中大约 12 种不同的芯片。但我们猜测，当涉及到支持更多芯片时，软件是一个限制因素。

通常 PIC 编程的问题是需要 12V 电源。他选择使用外部 12V 电源和 78L05 线性稳压器来获得 5V 供电轨。计算出功率后，需要考虑一些电平转换问题。RPi 在 GPIO 接头引脚上提供 3.3V 电压，但编程需要 5V 逻辑电平。他建立了晶体管和分压电路作为电平转换器。编程软件 bit 以每 1k 字编程数据不到 8 秒的写入时间撞击引脚。到目前为止，这还不能与 ICSP 一起工作，但他计划在未来的版本中添加这一功能。