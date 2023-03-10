# 闪存耐久性测试

> 原文：<https://hackaday.com/2014/12/04/flash-memory-endurance-testing/>

[基因]有一个项目，将大量设置写入 PIC 微控制器的闪存。闪存的读取/擦除周期有限，虽然这个明显的问题可以通过纠错码来缓解，但在选择特定 ECC 之前，最好先弄清楚闪存是如何出现故障的。现在的问题是不停地敲打图片直到它们呕吐出来，并找出这些芯片中闪存的故障模式。

这个实验的砧板上的芯片是一个 [PIC32MX150](http://www.microchip.com/wwwproducts/Devices.aspx?product=PIC32MX150F128B) ，有 128K 的 NOR 闪存和 3K 的额外闪存用于引导加载程序。硬件支持擦除所有闪存、擦除一页、编程一行和编程一个字。因为[Gene]希望有一位在失败后仍能工作，反之亦然，所以测试协议使用 RAM 缓冲区来比较闪存中测试的每一位的最新状态和新状态。一次测试 2K 的 RAM，总共 16K 的 Flash 可测试。代码基本上通过一个循环来擦除所有页(应该将所有位设置为“1”)，读取页以检查所有位是否为“1”，将“0”写入所有页，并读取页以检查所有位是否为“0”。测试的输出是一个 4.6 GB 的文本文件，看起来像这样:

```
Pass 723466, frame 0, offset 00000000, time 908b5feb, errors 824483 
ERROR: (E) offset 0000001E read FFFFFFFB desired FFFFFF7B.
ERROR: (E) offset 00000046 read FFFFFFFF desired 7FFFFFFF.
ERROR: (E) offset 00000084 read EFFFFFFF desired FFFFFFFF.
ERROR: (E) offset 0000008E read FFEFFFFF desired FFFFFFFF.
ERROR: (E) offset 000000B7 read FFFFFFDF desired FFFFFFFF.
ERROR: (E) offset 000000C4 read FFFBFFFF desired FFFFFFFF.
ERROR: (E) offset 000001B8 read FF7FFFFF desired 7F7FFFFF.
ERROR: (E) offset 000001BE read 7FFFFFFF desired FFFFFFFF.
ERROR: (E) offset 000001D2 read FFFFFF7F desired FFFFFFFF. 
Pass 723467, frame 0, offset 00000000, time 90aea31f, errors 824492 
ERROR: (E) offset 00000046 read 7FFFFFFF desired FFFFFFFF.

```

在该实验中测试的假设是，“每个位独立地可能失败，与擦除/写入周期的数量成指数关系”。有许多有趣的观察使[Gene]拒绝了这个假设:有数百万个擦除没有将一个位重置为‘1’的例子，但是没有一个写没有将一个‘1’位改变为‘0’的例子。这对开发纠错码方案来说非常好。

还有一种偏差，即一个字中的位会产生错误，与一个字中的其他位相比，位 31 和 32 更有可能出现错误。最令人费解的发现是每行失败次数的偏差:

![Graph5](img/7309d7fad9011c2d1d1f6e7f42130085.png)

PIC 中的一行闪存为 128 字节，如果所有行都有可能产生错误，那么上图会更无聊一些。很奇怪，[基因]不知道如何解释这些数据，只有解开其中一张照片并用显微镜观察才能告诉任何人为什么会这样。

至少，Microchip 严重低估了该微控制器上的闪存读取/擦除周期数；该芯片的额定循环次数为 20，000 次，第一个故障位出现在第 229，038 次循环中。在单独运行的情况下，第一次失败大约在第 400，000 次循环时。