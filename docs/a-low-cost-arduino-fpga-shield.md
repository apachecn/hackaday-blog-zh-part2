# 一种低成本 Arduino FPGA 屏蔽

> 原文：<https://hackaday.com/2014/03/05/a-low-cost-arduino-fpga-shield/>

[技术狂]在黑客项目上大放异彩。他正在创建一个[基于 Arduino 的低成本 FPGA 屏蔽](http://projects.hackaday.com/project/38/)。我们[在](http://hackaday.com/2011/07/17/fpga-arduino-shield-uses-kickstarted-as-a-preorder-system/)之前见过这种配对，但从未见过 25 到 30 美元范围内的材料清单。[技术狂的] [选择的 FPGA](http://en.wikipedia.org/wiki/Field-programmable_gate_array) 是 Xilinx [Spartan 6](http://www.xilinx.com/products/silicon-devices/fpga/spartan-6/) 。他还包括 SDRAM，以及用于配置的 SPI 闪存。尽管 Spartan 6 LX9 是一个相对较小的 FPGA，但它可以提供足够的冲击力，Arduino 几乎成为一个外设。两者之间的主要互连将是 Arduino 通过 SPI 对 Spartan 编程的能力。不过，由于共享的 I/O 引脚，并行工作流的空间是无限的。

[技术狂]在他的去耦原理图上花了不少时间。即使在相对较小的 FPGA 上，电源去耦也是一个大问题，尤其是当高速信号开始起作用时。谢天谢地，Xilinx 为这项任务提供了指南。我们不得不提到两个优秀的视频[技术狂]来解释他的设计。记录一个项目并不需要几个小时无休止的写作。有时，运行屏幕捕捉实用程序并单击“录制”会更简单。在撰写本文时，原理图刚刚被彻底检查过，在进入所有重要的布局阶段之前，[技术狂]正在寻求反馈。这个设计以 [Altium](http://www.altium.com/) 的格式出现在[他的 github 库](https://github.com/sfgit/FPGA_Arduino_Shield)上。由于其高成本，Altium 不是我们开放式硬件设计的首选。有免费的观看者，但是[技术狂]把他的原理图以 [PDF 格式](https://github.com/sfgit/FPGA_Arduino_Shield/blob/master/Design%20Files/Schematic/Arduino%20-%20FPGA%20Development%20Board.PDF?raw=true) (PDF 链接)上传，让它变得简单。为什么不去项目部帮帮他呢？

[https://www.youtube.com/embed/KOx5rO--3O0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/KOx5rO--3O0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/Qxtkg7UQqkg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/Qxtkg7UQqkg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)