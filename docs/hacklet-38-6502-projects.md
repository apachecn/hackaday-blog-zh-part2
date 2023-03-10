# hacklet 38–6502 项目

> 原文：<https://hackaday.com/2015/03/13/hacklet-38-6502-projects/>

6502 CPU 可能是所有 8 位处理器中最著名的，无论是家酿计算机的裸芯片形式，还是从 C64、NES 和 BBC Micro 中发现的稍加修改的衍生芯片。对于这一期的 Hacklet，我们来看看 hackaday.io 上所有基于 6502 的构建。

* * *

6502 上没有多少晶体管，非常适合在 FPGA 上实现。[Michael A. Morris]有一个 Arduino FPGA shield，他的 soft-6502 项目[叫做 Cameleon](http://hackaday.io/project/656-chameleon) 。板上有一堆 SPI 闪存和 FRAM，板上 128kB 的(并行)SRAM 足以处理您可以扔给它的任何计算任务。

由于 Cameleon 是基于可编程逻辑构建的，[Michael]认为将一些未使用的操作码用于是个好主意[。有用于协处理器支持的指令，以及一堆专门为使第四个实现](http://hackaday.io/project/656-chameleon/log/7133-m65c02a-instruction-set-enhancements)更容易而设计的指令。

* * *

![4244551421640813832](img/f4b3f3c225d376123403e999c8cf9c72.png)也许可编程逻辑不是你的菜，你会喜欢像俄亥俄科学或苹果 I 这样简单的计算机。[L-Star 是为你准备的](http://hackaday.io/project/3620-l-star-minimal-propeller6502-computer)。这是[Jac Goudsmit]的建造，以 6502、视差推进器为特色，其他几乎没有。

视差推进器是一个强大的(多核！)能够轻松处理视频输出、键盘输入以及为计算机的 ROM 和 RAM 提供服务的芯片。[Jac]的构建非常完美，如果您正在寻找在 6502 上运行代码的最简单方法，这就是您的方法。

* * *

6502 几乎无处不在，在逛当地电子垃圾回收店时，[他偶然发现了一些相当有趣的东西](http://hackaday.io/project/3874-getting-an-mtu-130-monomeg-board-running)。箱子上的徽章上写着“BS 医疗设备”，但在四处查看了一下后，他发现这是一个 MTU-130 系统，一台在当时显然是顶级产品的。

这台机器上有一些奇怪的东西——18 位寻址和 80kB 内存。到目前为止[Eric]已经设法转储了 ROM，他正在查看软驱控制器板，看看他是否能弄清楚它是如何映射的。弄清楚苹果 II 或 C64 上出了什么问题是一回事；这些都是有据可查的机器。弄清楚一台很少有人听说过的机器完全是另一回事，我们向[埃里克]和他的努力致敬。

* * *

![4000511410347834190](img/970e3473e26ebc0fc981759bc4ad95c6.png) [这是一个既有也没有 6502 的版本](http://hackaday.io/project/2993-shemachine)。【BladeRunner】的 SheMachine 是一台单板电脑，内置 65c816。816 是一个有趣的怪兽，它作为一个标准的 6502 操作，直到它的一个寄存器中的一位被翻转。之后，它有一个 24 位地址空间，用于寻址 16 兆字节的内存，16 位寄存器，但仍然完全向后兼容 6502。是的，它确实有奇怪的交错地址引脚，但我们只能想象如果这种芯片早几年问世，世界会是什么样子…

[BladeRunner]正在用 1MB 的 SRAM 设计 SheMachine 真的绰绰有余——并通过 CPLD 映射所有的内存。不管怎样，这就是你应该做的。