# 使用 OpenQCM 尽可能少地测量

> 原文：<https://hackaday.com/2015/03/31/measure-as-little-as-you-want-with-openqcm/>

[Novaetech SRL]的聪明人已经公开了 openQCM，他们的[开源石英晶体微量天平](http://openqcm.com)。QCM 利用石英晶体的压电特性测量非常微小的质量或质量变化。当一个物体被放置在该传感器的表面上时，可以检测到晶体共振频率的变化，并用于在各种实验条件下(空气、真空、液体)确定其质量。然而，大多数 QCM 技术是专有的，而且价格昂贵——微量天平本身至少要 3000 美元。任何消耗品，比如额外的水晶，都要多花几百美元。

openQCM 的灵敏度为 700 皮克。其核心是一个带有定制 PCB 的 Arduino Micro。电路板包含一个用于温度偏移读数的 10K 热敏电阻和一个用于 [Pierce 振荡器电路](http://en.wikipedia.org/wiki/Pierce_oscillator)的驱动器。石英晶体频率由[破解 Arduino 的 ATmega32u4 的定时器中断](http://openqcm.com/openqcm-has-arduino-inside-at-heart.html)决定。名为 FreqCount 的外部库使用时钟来计算 1 秒时间帧内 TTL 信号的脉冲数。这产生 1Hz 的石英晶体频率分辨率。用户界面是用 Java 构建的，因此可以在您的计算机上读取、绘制和存储数据。整个外壳是 3D 打印的，看起来传感器是没有外壳的标准振荡器晶体。

简单的设计使组装和维护变得轻而易举。它只有 55 克重。由于有夹子系统，更换石英晶体不需要特殊工具。openQCM 可以作为一个单元使用，也可以作为多个单元组成一个网络，满足您所有的精确测量需求。虽然他们提供的套件会花掉你 500 美元，但所有 3D 打印、组装和 PCB 的文件和原理图都可以在 openQCM 网站上免费获得。

[https://www.youtube.com/embed/kzmBK9mONq8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/kzmBK9mONq8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

【特别感谢 Augustineas 给我们发来这条提示！]