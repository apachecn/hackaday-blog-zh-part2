# 问黑客日:我们可能有一些 FPGAs 要黑

> 原文：<https://hackaday.com/2013/01/11/ask-hackaday-we-might-have-some-fpgas-to-hack/>

![rear](img/fc1270a45120d717446eee5ed56e37c3.png)

[Chris]是阿拉斯加一家医疗诊所的 IT 人员，直到最近，他监控、修复和用扳手敲打的系统包括 100 多个 Pano Logic“零客户机”瘦客户机。Pano Logic 刚刚倒闭，对这些小盒子的所有支持都被切断了，只剩下[Chris]一百多个非常有趣的硬件。

这些“零客户机”背后的想法是瘦客户机的理想——将所有的存储、处理、RAM 和其他东西都转移到服务器上。Pano Logic 比其他瘦客户机更进一步，去掉了 CPU、内存和瘦客户机中的所有东西。剩下的是一个 Spartan-6 FPGA、几个驱动 USB 端口的芯片、一对 HDMI 芯片和几个 DDR2 模块。基本上，[Chris]有大约 150 块 FPGA 开发板放在一个储藏室里。唯一需要的是一堆软件和极度的聪明。

在打开其中一个零客户端后，[Chris]在他认为是 6 引脚编程端口的旁边发现了一个 Spartan-6 FPGA。除了 FPGA 之外，还有一些其它芯片可以让任何 FPGA 开发板成为一个非常好用的工具:

*   [公羊](http://www.micron.com/parts/dram/ddr2-sdram/mt47h32m16hr-25e)
*   [以太网](http://octopart.com/partsearch#search/requestData&q=88E1119R)
*   [显示芯片](http://www.datasheetdir.com/CH7301C-TF-TR+DVI) (2)
*   [USB 控制器](http://www.smsc.com/index.php?pid=23&tid=140)
*   [音频芯片](http://www.alldatasheet.com/datasheet-pdf/pdf/169961/WOLFSON/WM8750BL.html)

我们同意[Chris]的观点，这些 Pano Logic zero 客户端显示出了很大的潜力。如果你想用一些废弃的硬件制作一个非常非常便宜的 FPGA 开发板，那么[去易趣](http://www.ebay.com/sch/i.html?_&_nkw=Pano+Logic+zero+client)或者和你当地的 IT 人员聊聊。