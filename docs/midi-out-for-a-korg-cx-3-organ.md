# 迷笛为 Korg CX-3 器官

> 原文：<https://hackaday.com/2013/04/27/midi-out-for-a-korg-cx-3-organ/>

![midi-out-for-a-vintage-korg-cx-3-organ](img/4bfbcd8a6d23cebfbc63059e2f3bd8ff.png)

[Michael]喜欢他的旧风琴，但最近他想知道是否有可能在不改变其原有功能的情况下添加 MIDI。通过一点研究和更多的努力，他完成了他的目标。

在这样一个高质量的硬件上工作的好处是你可以找到关于它们如何工作的资源(我们打赌这是为如何在它们坏了的时候修理它们而定制的)。[Michael]找到一个网站，上面有大量关于电路板及其工作原理的信息。由此，他能够找到几个芯片，这些芯片传输关于哪个键被按下的串行数据。答对了。

一旦他找到了这三个信号，他就做了一个板来把它们翻译成 MIDI 协议。他的电路是基于 ATtiny2313。它由线性电压调节器电路和缓冲芯片支持，后者将输入信号转换为所需的 5V 电平。他家的蚀刻板很干净，安装得很好，项目的成功可以在跳跃后的剪辑中听到。

[https://www.youtube.com/embed/xz96QpLLn74?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/xz96QpLLn74?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)