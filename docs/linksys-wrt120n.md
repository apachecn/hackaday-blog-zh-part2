# 入侵 Linksys WRT120N

> 原文：<https://hackaday.com/2014/02/07/linksys-wrt120n/>

[Craig Heffner]最近发现自己正在处理 Linksys WRT120N 路由器的[案例。路由器的固件使用了某种以前未知的混淆形式，这让那些希望运行自己软件的人感到头疼。WRT120N 是 2009 年的车型，在这一点上有点过时。然而，这并没有阻止[克雷格],他开始对固件混淆进行逆向工程。](http://www.devttys0.com/2014/02/reversing-the-wrt120n-firmware-obfuscation/)

[Craig]首先通过他自己的 [Binwalk 工具](http://binwalk.org/)运行固件。Binwalk 分析固件文件中的已知数据，无论是嵌入式文件系统、原始压缩流还是二进制文件。在这种情况下，Binwalk 只找到一个小的 LZMA 块，其中包含路由器 web 界面的压缩 html 文件。固件的其余部分是熵值很高的未知数据。【Craig】光靠固件更新文件做不了更多，于是他命令路由器从硬件端进攻。在里面，他发现了典型的低端路由器组件:一个 Atheros AR7240 SoC，一个 2MB SPI 闪存芯片，32MB RAM。他还发现了连环和 JTAG 的信头。

[Craig]连接到串行端口，看到一个引导菜单。这允许他在路由器上运行一些命令，但没有给他任何转储内存的方法。他必须直接找到来源——用一根 [FTDI C232HM](http://www.digikey.com/product-detail/en/C232HM-DDHSL-0/768-1106-ND/2714139) 电缆直接连接到路由器的 SPI 闪存。使用 [libmpsse](https://code.google.com/p/libmpsse/) ，他的另一个开源工具，【克雷格】能够转储闪存。他现在有了未混淆的引导程序代码，尽管是在 MIPS 汇编中。[Craig]然后就可以用 [IDA Pro](https://www.hex-rays.com/products/ida/index.shtml) 来追踪引导程序了。经过一番努力，混淆系统暴露了出来。该系统很简单，在 LZMA 标题块和数据的前几个字节之间进行了几次字节和半字节交换。[Craig]通过编写一个简单的 C 程序对固件进行去混淆和解压缩，完成了他的这部分工作。