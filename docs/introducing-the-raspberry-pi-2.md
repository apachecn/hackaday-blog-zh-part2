# 介绍树莓 Pi 2

> 原文：<https://hackaday.com/2015/02/02/introducing-the-raspberry-pi-2/>

***TL；T2 博士:它被称为树莓 Pi 2 型。四核 ARM Cortex A7，带 1g 内存。和树莓 Pi 型号 B+的外形一样。现已在纽瓦克、Element 14、Allied 和 RS Components 上市。和旧的价格一样。你不是孩子了，你应该学会阅读。***

* * *

三年前发布的最初的树莓派，当它第一次推出时，看起来有点老了。对于售价 35 美元的电脑来说，这是意料之中的。在电子世界里，三年是一段很长的时间，Pi 应该更新了。它现在就在这里，最大的变化是更快的四核芯片，更好的处理器架构和 1GB 的 RAM。

Raspberry Pi 2 Model B 采用四核 ARM Cortex A7，主频为 1GHz，内存为 1GB。该芯片采用 ARMv7 架构，而不是最初 Raspi 的 ARMv6。当我用它玩的时候，它明显比我几个月前的 Raspi Model B 在网页浏览任务上更快。非常非常酷，为 CPU 密集型应用打开了几扇大门。

虽然 CPU 已经更新，但 Pi 上没有太多其他变化。USB 和以太网仍由 LAN 9514 USB/以太网控制器处理。如果你正在寻找千兆以太网，很抱歉，那是不可能的。在这次硬件更新中，除了 CPU 之外，我们不会获得 eMMC 闪存、SATA 端口或任何突破性的东西。这几乎只是一个 CPU 和内存的升级。

在 Raspberry Pi 型号上找到的所有原始端口都在 Raspi 2 上找到；HDMI、音频、模拟视频、以太网、USB、CSI、目前未使用的 DSI 和 GPIO 端口没有变化。再一次，我们期待着这个硬件版本的 CPU 和 RAM 升级。

与以前的 Raspberry Pis 中 CPU 和 RAM 堆栈上的奇怪封装不同，RAM 现在移到了 Raspi 2 的后面:

[![raspiback](img/ac90ebe5bba58facc27c1dc239c8f6a8.png)](https://hackaday.com/wp-content/uploads/2015/02/raspiback1.jpg)

RAM 芯片是一个 [Elpida EDB8132B4PB-8D-F](http://www.micron.com/parts/dram/mobile-ddr2-sdram/edb8132b4pb-8d-f) ，一个 8gb DDR2 RAM，其时钟频率与原始 Raspi 中的 RAM 相同。不要指望内存性能或速度的提高。相反，你应该庆幸 Raspi 上现在有了一整千兆字节的内存。

你们中的一些人可能还记得那些树莓派早期采用者错过的“升级”。在第一批几十万个 Raspberry Pi 型号 b 发货后，有人[意识到他们可以将 RAM 从 256 MB 升级到 512 MB](http://hackaday.com/2012/10/15/raspis-with-double-the-ram-in-the-wild/) 。目前还不知道树莓 Pi 2 是否会如此轻松地升级。16 千兆位内存确实存在，但现在 CPU 和内存不在同一个封装上，有更多的问题需要考虑，而不仅仅是放下一个新的内存芯片。

### 和睦相处

就软件而言，几乎所有在最初的 Raspberry Pi 上运行的东西都可以在 Raspberry Pi 2 上运行。Raspberry Pi 2 的功能是原版的超集。这是一种全新的处理器架构；Pi 1 采用 ARMv6 架构的芯片，Cortex A7 采用 ARMv7 架构。这是巨大的。树莓 Pi 2 现在可以运行现代 Android 系统。π2 带来了无数π1 无法想象的可能性。

当涉及到 Pi 上的软件时，有一个警告。基金会给了我一个 Pi 2 和一个 SD 卡，里面装了一个 Raspbian 发行版。这工作得很好，直到我是一个白痴几次，切断电源的 Pi 2 没有做适当的关闭。该卡已损坏。我下载了一周前的拉斯扁图像。Pi 2 不会引导这个映像。如果你在用内核做一些事情，在 Pi 1 和 Pi 2 之间有*和*的区别，Pi 1 和 Pi 2 会有特定的磁盘映像。

有趣的是，Raspberry Pi 1 模型 B+将启动 Pi 2 的 Raspbian 映像。这有点有趣，因为 Pi 2 上的 CPU 实际上是 Pi 1 上 CPU 的超集。我和那些有着大约一个世纪 ARM 和 Linux 综合经验的人聊过，没人知道这是怎么回事。

对于硬件来说，你对 Raspberry Pi 上的 GPIO 引脚所期望的一切在 Raspberry Pi 2 上都有。这是我们都期待的常见 40 针扩展接口，据我所知，Raspi 和 Raspi 2 之间没有任何变化。

关于外形，几乎所有与 Raspberry Pi 兼容的机箱都应该与新的 Raspi 2 兼容。我用来自[哈蒙德](http://www.hammondmfg.com/1593HAM.htm#RaspPiBPLUS)、[卡姆登博斯](http://camdenboss.com/enclosures/raspberry-pi/raspberry-pi-b/raspberry-pi-b#raspberry-pi-b-enclosures)和[皮莫罗尼](http://shop.pimoroni.com/products/b-pibow-coupe)皮鲍轿跑的案例测试了新 Pi。只有 Pimoroni 与新的 Raspi 2 不兼容，但这只是因为一块丙烯酸树脂干扰了新的更大的 CPU。一对堤坝~~很快解决了这个问题~~把粉碎的丙烯酸树脂射到房间的另一边。使用薄锯或锉刀。就外形而言，这与 B+型完全相同。

### 其他型号

在 Raspberry Pi 生态系统中有不止一个 Pi，但目前，Model A+和 Raspberry Pi 计算模块将保留旧的 BCM2835 芯片组。这并不是说它们将来不会升级；围绕 CPU 和 RAM，Pi 1 型号 B+、A+和计算模块之间的板布局极其相似。对“较小的”Pis 的更新可能只是基金会使用的任何 EDA 软件的一个徒劳的问题。

历史上，Raspberry Pi 基金会一直将 B 型作为他们最先看到新创新的旗舰产品。当 [Model B+获得新的外形](http://hackaday.com/2014/07/14/the-raspberry-pi-model-b-is-here-again/)和更多的 GPIO 引脚后，[花了大约四个月](http://hackaday.com/2014/11/09/the-raspberry-pi-model-a/)Model A 才达到新的设计标准。如果您正在等待 A+或计算模块外形的 ARM Cortex A7 主板，您可能会等到 6 月或 7 月。

### 基准和性能

自从几年前推出 Raspberry Pi 以来，小型、廉价的 ARM Linux 主板出现了爆炸式增长。与[香蕉 Pi](http://www.bananapi.org/p/product.html) 、 [Cubieboard2](http://cubieboard.org/model/cb2/) 或 [Odroid](http://www.hardkernel.com/main/products/prdt_info.php) 相比，最初的树莓 Pi 中的 700MHz ARM11 CPU 在过去几年中似乎有点贫血。这不是树莓派的错；Raspberry Pi 的想法是以大约 35 美元的价格生产一台小型单板 Linux 计算机*。香蕉 Pi 和 Odroid 等“克隆”主板后来出现，它们可以获得更好、更便宜的硅，并且不受 35 美元价格的限制。总会有价格更高的更好的选择。*

树莓皮、“克隆”板与更大、更强、更贵的板如[鹰嘴豆板](http://www.solid-run.com/products/hummingboard/)和[比格犬骨黑](http://beagleboard.org/BLACK)之间的任何比较都必须考虑到板的价格。目前，很少有主板能够与 Raspberry Pi 2 的功率和价格相匹配，Odroid C1 在性能和功能方面可以与 Raspberry Pi 2 相匹配。不过，我没有 Odroid C1，我也不会打电话比较两者。

不过，我有一个树莓派 B+型号。明天，我将发布树莓 Pi 2 和树莓 Pi 模型 B+之间的一些基准测试。

**功率**

我刚好有一个 [FriedCircuits USB 电流/电压/功率计](http://store.hackaday.com/collections/products-tools/products/usb-tester-2-0)在身边。当监控 Raspi 2 的功耗时，其功耗比 Raspberry Pi 1 略有增加。

当引导到 Raspbian 桌面时，Raspberry Pi 1 消耗大约 290mA，一旦桌面被加载，则下降到大约 250mA。Raspberry Pi 2 在启动时消耗约 340mA，一旦加载桌面，消耗将降至约 270mA。从 Raspi 1 到 Raspi 2 的电流消耗略有增加。

通过一些实验，我确定树莓 Pi 2 在重负载下会消耗高达 500mA 的电流。这是 USB 的最大规格。如果你目前的 USB 电源适配器不是很好，你可能想为 Raspi 2 买一个更好的。

**速度**

明天我会发布一些关于 Raspberry Pi 2 的速度和基准的东西。在此之前，引导至桌面的时间可以作为 Raspberry Pi 2 中速度的充分表征。

在两次测试中使用相同的 SD 卡，Raspberry Pi 2 在 ***大约 22 秒*** 启动到 Raspbian 桌面。对于同样的测试，几个月大的 Raspberry Pi 1 型号 B+在 ***大约 41 秒*** 启动到 Raspbian 桌面。测试条件是“从 Tux 应该出现在控制台上的树莓出现的点”到“当屏幕角落的 CPU 监视器触底时”。以任何标准衡量，树莓 Pi 2 都要快得多。

### 哪里可以买到

任何参加过 Raspberry Pi 1 发布会的人都会记得纽瓦克、法内尔、Allied 和 RS components 长达数月的等待。这部分是由于巨大的需求，但缺货的很大一部分归咎于 Raspberry Pi 基金会。可以理解；当时，他们正期待着做梦也没想到的成功。

这一次，他们准备好了。[Eben]告诉我们现在有 100，000 台 Raspberry Pi 2 型号 b 在仓库里。新的 Pis 进入 Fry's 和 Microcenter 还需要一段时间，但我们预计要等几周，而不是最初推出的几个月。

### 总结

在很大程度上，这只是对 Raspberry Pi Model B 的 CPU 和 RAM 的升级。目前，还没有专门为 Raspberry Pi 2 编译的发行版或软件，拥有能够利用 Raspberry Pi 2 更快的多核 CPU 的软件还需要一段时间。

Raspi 2 更快更大的 CPU 为有趣的应用打开了几扇门。最初的 Raspberry Pi 有点贫血的 CPU 限制了小型 Linux 板的有趣应用。像计算机视觉这样的应用程序和任何需要大量 I/O 的应用程序都是不可能的。这个硬件版本将解决这个问题。

Raspberry Pi 的未来更新将包括模型 A+和计算模块。这些可能会在几个月后出现。你不会听到任何关于改进的树莓 Pi 2 或树莓 Pi 3 的消息。

明天将发布树莓 Pi 2 的详细分解和基准测试。

* * *

如果你在寻找“披露”这个词，它就在那里。在我的要求下，树莓派基金会给我发了一个树莓派 2 B 型和 SD 卡。