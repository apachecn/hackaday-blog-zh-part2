# Raspberry Pi 电源控制器增加了关断和启动功能

> 原文：<https://hackaday.com/2013/01/17/raspberry-pi-power-controller-adds-shutdown-and-startup-functionality/>

这个试验电路使用 PIC 芯片来控制 Raspberry Pi 的电源。当[我们围绕 RPi 板](http://hackaday.com/2012/11/19/raspberry-pi-reaches-critical-mass-as-xbmc-hardware/)建立了一个 XBMC 设置时，我们第一次注意到了 RPi 特性中的这个缺口。这并不是世界末日，但自从安装了树莓派后，我们每次使用后都会拔掉它。(凯文·桑吉里的)电路可能是实现这一过程自动化的途径。

这并不是真正针对媒体应用。PIC 电路确实将电源切换到 RPi，但目标是添加一个按钮来实现。该项目的其他目标包括计划关闭和电力轨上的电力不足事件的数据记录。正如您所看到的，在系统断电时，mix 中有一个硬币电池可以记录时间。RPi 通过 i2c 与 PIC 通信。这有助于使用 Linux 命令“shudown -h”完全关断，以及安排重启时间的能力。

增加一个红外接收器和调整 PIC 代码就可以从沙发上触发电源控制器。

[谢谢唐恩]