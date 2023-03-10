# 双端口 C64 闪光推车

> 原文：<https://hackaday.com/2014/12/26/dual-porting-a-c64-flash-cart/>

Commodore 64 的旧卡盒使用 EEPROMs 来存储数据，而较新的闪存卡使用闪存芯片或 SD 卡来将一大堆游戏放在一个小塑料砖中。[Stian]和[Runar]认为这还不够好——他们想对墨盒进行实时编程，在不接触 C64 的情况下重新启动它的能力，以及用于编码和测试的设备。他们想出的是 Commodore 弹药筒技术的最新进展。

该设备为 C64 提供 8k 内存，但它不使用闪存或 EEPROM。相反，[Stian]和[Runar]使用的是双端口静态 RAM，具体来说就是来自 IDT7005 系列的[一个。该芯片有两条数据总线、两条地址总线和/CE、/OE 和 R/W 线，用于芯片的任一侧，允许其他数字电路连接到 C64 存储器的一小部分。](http://www.datasheet.net/search?q=idt7005s55pf)

购物车中还有一台运行 V-USB 的 ATmega16，用于处理 PC 通信。大约需要 1 到 1.5 秒的时间将整个 8k 传输到盒式磁盘上，但是这个芯片可以同时读写 RAM 和 C64。

如果你想要一个盒子，它能让你在一个盒子里装上所有的游戏，这不是你想要的。但是，如果你想写一些 C64 游戏，做一些现场调试，这是一个适合你的。Eagle 文件是可用的，下面有一个视频演示。

[https://www.youtube.com/embed/vt_Jcx0B2do?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/vt_Jcx0B2do?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)