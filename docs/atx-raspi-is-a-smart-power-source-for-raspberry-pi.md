# ATX Raspi 是树莓派的智能电源

> 原文：<https://hackaday.com/2013/05/19/atx-raspi-is-a-smart-power-source-for-raspberry-pi/>

树莓派一直挑战我们的一个方面就是电源。从标准的微型 USB 端口为主板供电是一个好主意，因为规模经济使得手机充电器(即使在 RPi 稳定运行所需的 1A 范围内)便宜且容易获得。我们缺少的是使用内置硬件来开启和关闭设备的能力。这一困境引发了许多不同的解决方案，ATX 拉斯比智能 PSU 是我们遇到的最好的一个。这是对今年早些时候我们看到的基于 PIC 的版本[的一个很好的打包。](http://hackaday.com/2013/01/17/raspberry-pi-power-controller-adds-shutdown-and-startup-functionality/)

该器件是一个小型 PCB，充当 micro-USB 电源和 RPi 板之间的桥梁。它提供了几个分接头，其中一个用于电源按钮。该按钮由微控制器监控，微控制器相应地切换车载继电器。但它不会在你想关机的时候切断电源。它首先向 RPi GPIO 引脚之一发送信号，导致操作系统执行关机脚本。然后，它监视 RPi，以便在切断电源之前完成关机任务。

[https://www.youtube.com/embed/lM_fUPE9Lm8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/lM_fUPE9Lm8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)