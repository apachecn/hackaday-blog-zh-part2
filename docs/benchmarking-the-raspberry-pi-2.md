# 树莓 Pi 2 的基准测试

> 原文：<https://hackaday.com/2015/02/05/benchmarking-the-raspberry-pi-2/>

树莓派上市才几天，但这些电路板已经通过邮局，出现在世界各地的工作台上。[从最初的印象](http://hackaday.com/2015/02/02/introducing-the-raspberry-pi-2/)来看，我们已经知道这款四核 ARMv7 系统的启动时间只有一半，但除此之外，没有多少真正的基准测试将新的 Raspberry Pi 2 与旧的 Raspi 1 或其他类似的小型 Linux 开发板进行比较。这篇文章解决了这个问题。

但是，有一个警告:这些是基准，基准不是真实世界的用例。然而，我们可以通过一些简单的工具收集一些关于 Raspberry Pi 2 真实性能的信息。

在这些测试中，我使用了罗伊·隆巴顿的 Raspberry Pi 基准测试工具、 [nbench](http://www.tux.org/~mayer/linux/bmark.html) 和一些定制工具来确定两种硬件版本的 Raspberry 在真实用例中的速度。

#### 双精度 Linpack

```
Raspberry Pi Model B+ (700 MHz):    40.64 Mflops
Raspberry Pi 2 Model B (1000 MHz)*: 92.88 Mflops

*using one core

```

#### Dhrystone 版本 2.1

```
Raspberry Pi Model B+ (700 MHz):    Dhrystones per Second: 1481481
                                    VAX MIPS rating = 843.19
Raspberry Pi 2 Model B (1000 MHz)*: Dhrystones per Second: 2085024
                                    VAX MIPS rating = 1186.70

*using one core

```

#### OpenGL

如果 Raspberry Pi 2 的图形功能有所改进，会有一些问题。幸运的是，[我们可以很容易地测试这个](http://www.roylongbottom.org.uk/Raspberry%20Pi%20Benchmarks.htm#anchor18)。正如所料，Raspi 1 和 Raspi 2 的 OpenGL 功能没有明显的区别。两个测试都在 1280×720 分辨率下运行:

```
Raspberry Pi Model B+ (700 MHz):
                                 Triangles WireFrame Shaded Shaded+ Textured
                                 900+      120.02    120.01 84.77   76.70
                                 9000+     39.23     39.16  29.29   22.75
                                 18000+    19.91     19.86  16.98   12.67
                                 36000+    9.98      10.00  9.21    6.68

Raspberry Pi 2 Model B (1000 MHz)*:
                                 Triangles WireFrame Shaded Shaded+ Textured
                                 900+      120.10    120.00 88.26   80.84
                                 9000+     40.77     40.61  30.45   24.19
                                 18000+    20.68     20.62  17.64   13.63
                                 36000+    10.39     10.37  9.57    7.35
*using one core

```

#### 单核 Python 性能

最后，一个真实的用例。能够在 Python 中快速处理事情是树莓 Pi 酷的一大部分，有一个简单的、有点标准的方法来解决这个问题:[找到所有小于一百万的质数](http://www.raspberrypi-spy.co.uk/2012/06/overclocking-benchmarking-the-raspberry-pi/)。这两个测试都是用 Python 2 运行的。Raspberry Pi 2 只使用了一个内核。Raspi 2 最终的速度是 Raspi 1 的两倍多；Raspi 1 在 51 分钟内完成了任务，Raspi 2 在 21 分钟内完成。

```
Raspberry Pi Model B+ (700 MHz):
found 78497 primes under 1 million in 51:32.034

Raspberry Pi 2 Model B (1000 MHz)*:
found 78497 primes under 1 million in 21:19.825

*using one core

```

### 拉斯皮 2 对比格犬骨黑

每个人都在等待的战斗。截至一周前，如果你想要一个权力相对较高的董事会，拥有一个伟大的社区，你正在寻找 BeagleBone。现在，没那么多了。借助 nbench，Raspi 2 的单核性能可与 BeagleBone Black 媲美:

#### nbench

```
Raspberry Pi Model B+ (700 MHz):
                                 INTEGER INDEX :        16.100
                                 FLOATING-POINT INDEX : 5.568

Raspberry Pi 2 Model B (1000 MHz)*:
                                 INTEGER INDEX :        22.322
                                 FLOATING-POINT INDEX:  9.578

BeagleBone Black (1000 MHz):
                                 INTEGER INDEX :        23.314
                                 FLOATING-POINT INDEX:  2.976
*using one core

```

对于整数性能，Raspi 2 手击败 Raspi 1。Raspi 2 和 BB 黑不相上下。BeagleBone Black 上的浮点异常低，我要把这归咎于我没有正确设置编译器选项。

#### 我应该放在 led 里的东西

复古控制台仿真！*马里奥卡丁车*和*时间的陶笛*和*骗子的恶毛日*！没有人真的用树莓派来制造东西，这只是一种奇怪的怀旧消费主义，包裹在一种流行的“制造”潮流中！

最初的 Raspberry Pi 看到了许多模拟器的使用，但它是有限的:Pi 1 可以轻松处理 NES，SNES，Genesis/Mega Drive 和其他早期的控制台。N64 和原始 Playstation 游戏的模拟器性能*几乎*无法播放。现在，Raspi 2 可以轻松处理 N64 和 PSX 游戏。【HoZyVN】[试玩了 N64 的*马里奥卡丁车*](https://www.youtube.com/watch?v=tP-i6oM2vnQ) 和 [PSX 的*斯皮罗龙*](https://www.youtube.com/watch?v=7rBaId0CfqM) 。它们是可以玩的，整整一代人都涌向 Microcenter，重温他们整天坐在控制台电视前喝着 Sunny D 的光辉岁月。

#### 结论

最初的 Raspberry Pi 是一个有趣的教育工具，但它不是一台可用的计算机。我用了一个 Raspi 1 当工作台电脑用了一个星期左右。很慢，很糟糕。Raspberry Pi 2 作为一个小巧、廉价、便携的桌面系统非常有用，增加的功能为 35 美元的电脑打开了几扇大门。

当你考虑到社区对 Raspberry Pi 的支持，Github 上数以千计的随机库，以及大量已经存在的用于 Raspberry Pi 的主板时，这可能是目前最好的小型 Linux 主板。如果你需要更强大的东西，你将会升级到“真正的”笔记本电脑或台式机。