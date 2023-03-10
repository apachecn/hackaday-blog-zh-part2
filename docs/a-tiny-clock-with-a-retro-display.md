# 带有复古显示屏的小时钟

> 原文：<https://hackaday.com/2014/01/08/a-tiny-clock-with-a-retro-display/>

[![](img/4567713a52ad6d4d53dabcc0f34816c1.png)](http://hackaday.com/wp-content/uploads/2014/01/hpdl-1414-clock-top.jpg)

在将 Contiki 移植到他的 TI Launchpad 平台后，[Marcus]渴望用它做点什么。因此他[用老式](http://www.bithappens.se/blog/2013/05/26/clock-with-retro-display/) [HPDL-1414](http://www.farnell.com/datasheets/76528.pdf) “智能四字符 16 段字母数字显示器”和 msp430g2553 制造了一个简单的时钟。

你可以看到上面的结果是通过 USB 供电，包括一个 3.3V LDO 线性稳压器以及一个按钮，一个 LED，一个晶体和几个无源组件。幸运的是，5V 供电的 HPDL-1414 显示器在其输入端接受 3.3V 逻辑，避免了对电平转换器的需要。

时钟程序运行在移植的 Contiki 2.6 上，你可以在他的 [Github 库](https://github.com/msloth/contiki-launchpad)上找到。[马库斯]正在考虑在上班时间使用振动马达，每隔 20 分钟嗡嗡响一次，以提醒人们遵守 20-20-20 法则来对抗眼睛疲劳:每隔 20 分钟，看 20 英尺外的东西 20 秒钟。在休息之后嵌入了该系统运行的视频。

[https://www.youtube.com/embed/H-n53o-2VUA?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/H-n53o-2VUA?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)