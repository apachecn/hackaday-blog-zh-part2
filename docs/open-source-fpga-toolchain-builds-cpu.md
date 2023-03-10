# 开源 FPGA 工具链构建 CPU

> 原文：<https://hackaday.com/2015/07/28/open-source-fpga-toolchain-builds-cpu/>

当你开发软件时，你需要某种工具链。比如为 ARM 处理器开发，你需要一个合适的 C 编译器，一个链接器，一个库，一个程序员。FPGAs 使用一套类似的工具。然而，这些工具不是将源代码转换为机器语言，而是将源代码的意图映射到 FPGA 元素的配置以及它们之间的连接。

有一些变化，但 FPGA 构建的基本流程是使用合成器将 Verilog 或 VHDL 转换为物理设计。然后，映射器将该设计映射到特定 FPGA 上可用的物理元件。最后，布局和布线步骤决定了如何将这些元素相互连接起来。最后一步是生成芯片能够理解的比特流，并以某种方式将其加载到芯片中(通常通过 JTAG 或对芯片或外部 EEPROM 编程)。

自制工具的一个问题是，制造商通常对比特流格式和其他重要细节知之甚少。当然，任何事情都可以被逆向工程(很困难)，而且[James Bowman]能够使用开源网格工具链[构建一个最小的 CPU](http://www.excamera.com/sphinx/article-j1a-swapforth.html) 。该项目依赖于几个开源项目，包括为 Lattice iCE40 FPGAs 提供配置工具的 [IceStorm](http://www.clifford.at/icestorm/) (有一个[非常便宜的开发平台可用于该设备](http://www.latticesemi.com/icestick))。

在之前，我们已经报道过冰风暴。IceStorm 项目提供了三个工具:一个从 ASCII 表示产生芯片的二进制格式(和反向转换)，一个用于 iCEstick 和 HX8K 开发板的程序员，以及告诉其他开源工具关于该设备的数据库。

这些工具与其他开源工具融合在一起，形成了一个完整的工具链——这是开源协作的一个很好的例子。Yosys 进行合成(EDAPlayground 网站上的[工具之一)。《地点和路线》是由阿拉克尼完成的。组合工具现在足以构建 J1A CPU，甚至可以运行 Forth 的简单版本。如果你曾经想玩基于 FPGA 的 CPU 设计，你现在有一个 22 美元的硬件选项和免费工具。](http://hackaday.com/2015/07/21/learn-fpgas-in-your-browser/)

[https://www.youtube.com/embed/rdLgLCIDSk0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/rdLgLCIDSk0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)