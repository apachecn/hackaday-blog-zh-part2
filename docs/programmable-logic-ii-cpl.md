# 可编程逻辑 II–CPL

> 原文：<https://hackaday.com/2014/06/25/programmable-logic-ii-cpl/>

[https://www.youtube.com/embed/X28s0zHMVwM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/X28s0zHMVwM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

复杂可编程逻辑器件(CPLD)是现场可编程逻辑阵列(FPLA)的小表弟，有各种各样的廉价开发(dev)板

使用廉价的电路板和从 Xilinx 和 Altera 等主要可编程公司免费下载的开发软件，唯一需要的额外东西是一个编程器模块。易趣上有便宜的，但我希望有人花时间教 ARM/Arduino 成为程序员。

我有一个开发板的小集合，包括一些易趣特价和几年前我做的设计供选择。因为今天我要拿一个还没有完全检验过的较新的板子；一台 Altera Max V 设备。我已经塞满了 CPLD，时钟振荡器，一些 LED 和部分板载电源以及编程 CPLD 所需的 JTAG 头，仅此而已。

[![Herdware CPLD 5M570ZT](img/91e99ecbb0c1ce17d60e9598074a2e58.png)](http://hackaday.com/wp-content/uploads/2014/06/cpld.png)

Herdware CPLD 5M570ZT dedicated PCB with SRAM.

[![CPLD Schematic](img/81a59d5ee1890fdde6c2f2cab2dfe399.png)](http://hackaday.com/wp-content/uploads/2014/06/cpld-schematic.png)

CPLD Schematic showing an Altera CPLD 5M570T144

在外面，重要的信号是一个主时钟(没有时钟什么都不会发生)，然后是 LED 输出，让我们知道正在发生什么。在过去的 TTL 时代，你通常不能直接驱动 LED，所以这种能力本身就是时代的标志。

从时钟输入开始，你可以看到下面的引脚和振荡器。我们将使用软件中的可设置参数将该输入连接到低偏斜全局时钟(gclk)分配网络。时钟到达整个器件中不同寄存器的时间差异称为偏斜，如果它明显晚于或早于某些模块，可能会对逻辑产生严重影响。(当所有其他数据都锁存当前数据时，锁存旧数据或中间数据。

[![schematic2](img/49fb11bd93e62a41f0aa6ff00e31906b.png)](http://hackaday.com/wp-content/uploads/2014/06/schematic2.png)

时钟流中的 22 欧姆电阻放置在振荡器附近，匹配阻抗并吸收反射，但在不同的视频中会有更多内容。

一旦时钟进入设备，我们需要将它连接到全局时钟。这是在原理图层面完成的，我选择在顶层使用原理图，通过添加一个标记为 Global 的原语。如果使用 HDL 语言，你也应该指定一个全局原语。

[![gclk zoom](img/14a16dea25e2bf5ab97ae5c5e88d6e50.png)](http://hackaday.com/wp-content/uploads/2014/06/gclk-zoom.png)

一旦连接到全球时钟，还有不同区域的辅助时钟和“区域”时钟，如下所示:

[![Global Clock Distibution](img/42f0d1535a725906576c38bf4b774ee5.png)](http://hackaday.com/wp-content/uploads/2014/06/gclk.png)

Altera Global Clock Distibution

上图过于简化，Altera Max 的一个逻辑模块实际上如下图所示。

[![Altera LE MAX V Logic Block](img/2fb698f34eee7a356a03f874c81f7cce.png)](http://hackaday.com/wp-content/uploads/2014/06/altera-le-pnh.png)

Altera LE MAX V Logic Block

生活在芯片上的一个非常重要的概念是，试图预测最小延迟是不安全的，附近硅中的门非常快，简单的逻辑可能会传播故障或未知。所有这些问题都会影响使用组合逻辑驱动时钟输入的适用性。一种好的技术是进行大量的计算，然后停下来用全局时钟将结果保存在寄存器中，这种技术被称为流水线技术

恢复时钟驱动的一个例子可能是这样的，用于检测上升沿。

[![no-async](img/38a9d6ec6458d1c313c82dae54968768.png)](http://hackaday.com/wp-content/uploads/2014/06/no-async.png)

在某种程度上，我们需要与外界接触。在高利用率设计中，PCB 布局会一直等到可编程逻辑显著完成，至少是在引脚分配永久冻结的情况下仍可编译(编译器喜欢选择自己的引脚)。在我的情况下，我已经冻结了引脚，当我设计的 PCB 和分配可以在这里看到。

[![schematic1](img/a75661d867edbc4c10626e9139e7e558.png)](http://hackaday.com/wp-content/uploads/2014/06/schematic1.png)

[![schematic2](img/49fb11bd93e62a41f0aa6ff00e31906b.png)](http://hackaday.com/wp-content/uploads/2014/06/schematic2.png)

我给管脚命名是为了反映与 PCB 匹配的管脚号，这样我可以很容易地从内部连接管脚。

[![CPLD Device showing assignments.](img/f536b9b39b30fab81cf8849b94b407ed.png)](http://hackaday.com/wp-content/uploads/2014/06/altera2.png)

CPLD Device showing assignments.

正如我所提到的，我喜欢在设计的顶层有一个示意图，我在那里做任何尺寸或反转，因为对于像我这样的恐龙来说，这更直观。当用 64 位计数器将 50Mhz 时钟分频成可见的东西时，我们的设计看起来会是这样。

[![ncounter](img/bc3b0d2cd9ac8ef2b89928af617f2ca9.png)](http://hackaday.com/wp-content/uploads/2014/06/ncounter.png) 我们还没有定义计数器，我称之为 ncounter，因为我会根据我设置的参数把它变大 n 位。使用一个编辑器和我剩下的九个手指，我创建了这个过于简单的文件。我说过于简单是因为我没有包括重置和其他有助于物理和模拟结果的内务逻辑(我说九个手指是因为我去年夏天撕掉了一个)。

[![Verilog Programmable Width Counter](img/66133f5048a0697d53df3b651c958302.png)](http://hackaday.com/wp-content/uploads/2014/06/verilog-ncounter.png)

Verilog Programmable Width Counter

输入并保存后，单击会导致“创建符号”命令运行，并创建计数器符号。设置宽度的参数默认为 7 (8 位)，但会被从顶层向下推的 64 位所覆盖。

最后，我会简单介绍一下我是如何处理 Max V 器件的内核电压为 1.8v 这一事实的，我选择在 3.3V 下运行接口引脚，使其成为双电压器件。我用 Labcenter 的 Proteus 做原理图和 PCB(248 美元)，它的一个优点是它有一个强大的自动布线器，布线速度比我更快更好。我不手工布线，因为不可避免地会有变化，重新布线所花的时间是我没有的时间。因此，本质上我教(约束)自动路由器如何做得更好，每一个连续的通道。

[![cpld shield PCB](img/28e616e076bac40197312e6805d65549.png)](http://hackaday.com/wp-content/uploads/2014/06/cpld-shield-pcb.png)

CPLD Shield top and bottom layer

这是一个 4 层板，第二层(从上往下)是地，第三层是+3.3V，因为它也被外围芯片使用。这就需要为 CPLD 路由核心 1.8V 电源。

如下图所示，我为 1.8V 电源创建了一个环形电源路径，两个内层上有几个内部互连。我经常跳层，以便接地返回(和+3.3)电流可以沿着直线路径到达源极，而不必绕来绕去寻找退出路径。此外，中心保持较低的阻抗，而不是被几乎四面包围而被隔离。有一个环路可以降低 DC 和交流电阻，因为不仅有并行路径在工作，而且没有东西可以反射。存根通常是坏的。

[![1.8v route on inner layers without stubs](img/6de133e6fcb6fa286ad3caf8348cabb7.png)](http://hackaday.com/wp-content/uploads/2014/06/1-8v-route.png)

1.8v route on inner layers without stubs

使用内置在软件中的编程器，我在编译代码后上传代码，led 灯闪烁。你不用相信我的话，你可以看视频…我保证工作中很少有 CGI。

虽然这只是最简短的演练，但如果您跟随学习，您会体验到 CPLD 甚至 FPGA 编程的所有步骤。

我在考虑采用这种版本的 PCB，它不仅具有快速 SRAM，还具有电压电平转换器，允许接口达到 5v 等电压。一种想法是制作 Arduino 驱动的逻辑分析仪，因为 Arduino 不需要“高速”运行，CPLD 硬件会处理所有这些。