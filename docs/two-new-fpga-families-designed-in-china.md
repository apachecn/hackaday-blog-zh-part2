# 两个新的 FPGA 系列，在中国设计

> 原文：<https://hackaday.com/2015/08/24/two-new-fpga-families-designed-in-china/>

到目前为止，最大的两家 FPGAs 制造商是 Altera 和 Xilinx。他们控制了 80%以上的市场份额，而 Lattice 和其他公司占据了市场的最后部分。这种影响在 EE 实验室和阿里巴巴就可以看出来；几乎每一个 FPGA 开发板、每一个教学和每一点课程都基于 Altera 或 Xilinx 芯片。

东部出现了新的竞争者。高文半导体[在不到两年的时间里发布了两行 FPGA](http://www.gowinsemi.com.cn/newsshow.aspx?n_id=317)([谷歌翻译](https://translate.google.com/translate?sl=zh-CN&tl=en&js=y&prev=_t&hl=en&ie=UTF-8&u=http%3A%2F%2Fwww.gowinsemi.com.cn%2Fnewsshow.aspx%3Fn_id%3D317&edit-text=&act=url))。对于一家似乎正准备挑战 Altera 和 Xilinx monolith 的公司来说，这是令人难以置信的快。

上周发布的 FPGA 系列 GW1N 系列由两款器件组成，分别具有 1，152 和 8，640 个 lut。这些 FPGAs 基于 55 纳米工艺制造，旨在与 Altera 和 Xilinx 的低端产品竞争。这增加了 Gowin 去年 5 月推出的 GW2A ( [谷歌翻译](https://translate.google.com/translate?sl=zh-CN&tl=en&js=y&prev=_t&hl=en&ie=UTF-8&u=http%3A%2F%2Fwww.gowinsemi.com.cn%2Fnewsshow.aspx%3Fn_id%3D295&edit-text=&act=url))系列的产品组合[，其特点是设备从 18，000 到 55，000 个 lut 和 DSP 模块。封装种类繁多，从易于焊接的 QFN32 和 LQFP100，到引脚数量超过皇家舞会上 18 世纪女裁缝的 BGA 封装。](http://www.gowinsemi.com.cn/newsshow.aspx?n_id=295)

相比之下，Xilinx 的 Spartan-6 LX 系列从具有 3，840 个 lut 和 216kb 块 RAM 的设备开始，更大的设备具有 147，443 个 lut 和高达 268kb 的块 RAM。Altera 的 Cyclone IV E 设备也有类似的配备，设备从 6，272 到 114，480 lut 不等。在 Gowin 最近推出的两个器件系列之间，几乎涵盖了低端 FPGAs 的整个市场，并且它们在当前产品的基础上有所改进:GW1N 芯片具有随机存取片上闪存。Altera 的低端设备和 Lattice 的设备都不提供随机存取闪存。

Gowin 新 FPGAs 的工具链几乎完全基于 [Synopsys 的 Synplify Pro](http://www.synopsys.com/Tools/Implementation/FPGAImplementation/FPGASynthesis/Pages/SynplifyPro.aspx) ，使用 Gowin 的专用工具将 HDL 转换为芯片的比特流。这笔交易[是去年](http://news.synopsys.com/2014-10-27-Synopsys-and-Gowin-Semiconductor-Ink-Multi-Year-OEM-Agreement-for-FPGA-Design-Software)签订的。至于这些设备何时上市，Gowin 希望很快将套件发送给合格的开发者，这些设备可能很快就会出现在分销商的仓库中。

与绝大多数 FPGA 不同，高云的 FPGA 是在中国设计和制造的。这使得高文在这片万物皆产的土地上拥有独一无二的主场优势。凭借这些 FPGAs 可以处理的 LVDS、DSP 和其他外设，Gowin 的产品为距离 Gowin 工厂几英里远的开发人员和产品工程师提供了多种选择。

就 FPGA 而言，GW1N 和 GW2A 系列相当小。不过，这种限制是由容量决定的，而不是由发货数量决定的。FPGAs 的最大市场将是消费品，这几乎是同义反复，Gowin 在深入高端设计之前，专注于销售良好的产品。我们将很快看到这些芯片出现在设备中，随之而来的是一个可以修补的新平台。

如果你想在开源硬件和软件的世界上留下你的印记，你可以做得比开始挖掘这些 Gowin 芯片的合成和比特流更糟。就在几个月前， [Lattice 的 iCE40 位流被逆向工程](http://hackaday.com/2015/03/29/reverse-engineering-lattices-ice40-fpga-bitstream/)，已经有一些电路板利用完全开源的可编程逻辑工具链。随着更多有能力的 FPGAs 从中国出来，可以被塞进任何可以想象的产品中，这对硬件黑客和开发者来说都是一个黄金机会。

[谢谢你的提示 Antti]