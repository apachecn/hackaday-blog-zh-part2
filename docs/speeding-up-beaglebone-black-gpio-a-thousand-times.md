# 将 BeagleBone Black GPIO 加速一千倍

> 原文：<https://hackaday.com/2013/12/07/speeding-up-beaglebone-black-gpio-a-thousand-times/>

对于 Raspberry Pi 和 BeagleBone Black 来说，都有大量的 GPIO 访问，就像普通的 Unix 系统一样——通过移动文件。是的，对于大多数应用程序来说，你真的不需要非常快的 GPIO，但是在你需要的时候，使用/sysfs 是不行的。

[Chirag]正在摆弄一个猎兔犬骨和一个正交编码器，发现通常的戳戳针的方法不起作用。通过将他的示波器连接到一个用/sysfs 开关的引脚，他发现——令他震惊的是 BBB 的 GPIO 的最大速度约为 3.5 千赫。必须做点什么。

在发现[一个旧的堆栈溢出问题](http://stackoverflow.com/questions/13124271/driving-beaglebone-gpio-through-dev-mem)后，【Chirag】想到了使用/dev/mem 来切换他的管脚的解决方案。用示波器快速检查后发现，他现在以 2.8 兆赫的频率切换引脚，比以前快了大约 1000 倍。