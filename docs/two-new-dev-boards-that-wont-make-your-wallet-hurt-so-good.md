# 两个不会让你的钱包受伤的新开发板-太好了

> 原文：<https://hackaday.com/2015/06/13/two-new-dev-boards-that-wont-make-your-wallet-hurt-so-good/>

如果你一直关注爱好者 FPGA 社区，你会认为 DE0 Nano 是“小型 FPGA”，拥有从 [Oldland cpu 内核](http://hackaday.com/2015/03/20/the-oldland-cpu-32-bit-fpga-core/)到可合成[视差推进器处理器](http://hackaday.com/2014/08/07/parallax-propeller-1-goes-open-source/)的深厚项目历史。在这个领域工作了四年多之后，是时候重新开始了。

它的继任者 [DE0 Nano SoC](http://www.terasic.com.tw/cgi-bin/page/archive.pl?Language=English&No=941) 从多个角度进行了彻底的重新设计，同时尽最大努力保留了第一款如此吸引人的小巧外形和价格。首先，开发板拥有一个具有 40，000 个逻辑元件(高于 DE0 的 22K)的 Cyclone V 和一个集成的双核 Arm Cortex A9 处理器。PCB 布局还通过母接头为我们带来了 3.3V Arduino 屏蔽兼容性，1 Gig 外部 DDR3 SDRAM 和通过两个板载 ASICs 处理协议的千兆以太网支持。Terasic 的人似乎也在向“Duino-Pi”爱好者社区脱帽致敬，因为他们友好地提供了 [Linux 和 Arduino 映像](http://www.terasic.com/downloads/cd-rom/de0-nano-soc/)，让你在经典有限状态机和日常组合逻辑的基础上更上一层楼。

虽然新的 SoC 型号的外形尺寸略大，为 68.59 毫米 x 96mm 毫米(而不是原来的 49 毫米 x 75.2mm 毫米)，但我们要说的是，对于逻辑层面的新可能性来说，这只是一个小小的代价。这款主板现在在网上上架，售价 100 美元。

接下来，作为提醒，前面提到的 Arduino Zero 终于在 6 月 15 日发布了。如果你曾经考虑过从 8 位处理器跳到 32 位处理器，而不需要费力地设置 ARM 工具链，现在可能是开始的好时机。

via[[Arduino 博客](http://blog.arduino.cc/2015/06/10/arduino-zero-for-purchase-15th-june/)