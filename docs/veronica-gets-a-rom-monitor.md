# 维罗妮卡得到一个只读存储器监视器

> 原文：<https://hackaday.com/2014/01/28/veronica-gets-a-rom-monitor/>

![monitor](img/004625d1f3920eee1918564e2a8ee93b.png)

[Quinn]在 Veronica 上已经有一段时间了，她基于 6502 的计算机，但直到最近，它更多的是一个嵌入式项目，而不是一个全功能的计算机。在上为维罗妮卡*写软件维罗妮卡从一开始就是目标，最后[【奎因】可以从 rom 监控器](http://quinndunki.com/blondihacks/?p=1547)上写代码。*

在最基本的状态下，ROM 监视器是一个非常简单的软件。它驻留在计算机的 ROM 中，是计算机启动时加载的第一个东西，允许用户检查、读取和写入内存位置，以十六进制编写代码，并直接从监视器运行它。

为了编写 ROM 监视器(和其他一些程序)，[Quinn]正在使用令人敬畏的 [cc65 6502 C 编译器](http://www.cc65.org/)。它附带了一大堆宏，可以轻松读取键盘输入，将数据存入 AVR GPU，并写入内存。监控程序加载到她的 ROM 芯片上，每次按下复位按钮时，该芯片都会自动读取。

在下面的视频中，你可以看到[Quinn]写了几个位到地址$2000，告诉 CPU 输出 ASCII 字符到显示器。虽然不多，但这是[Quinn]第一次在 Veronica 上为 Veronica 编写代码，应该会被证明是一个非常有趣的系统的开端。

[https://www.youtube.com/embed/X6tn0mxHetY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/X6tn0mxHetY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)