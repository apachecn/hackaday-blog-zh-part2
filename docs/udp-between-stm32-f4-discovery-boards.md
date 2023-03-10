# STM32-F4 发现板之间的 UDP

> 原文：<https://hackaday.com/2013/02/15/udp-between-stm32-f4-discovery-boards/>

![stm32-f4-udp](img/6aca6e07771221199ce5ef17d004aa1f.png)

[边远地区的工程师]为 STM32-F4 探索板测试了一个新的附件套件。上图显示[两块板通过 UDP 协议](http://www.backwoodsengineer.com/2013/02/geeky-post-stm32f4-bb-ethernet-projects.html)进行通信。请注意每个发现板插入的额外 PCB。这是[一个第三方插件](http://www.embedinfo.com/english/product/DM-STF4BB.asp)，它增加了以太网、RS-232、SD 卡插槽和一个用于 LCD 或相机的连接器。我们手头有一个 F4 发现板已经有一段时间了，但还没有找到将外部硬件连接到巨大的双引脚接头的好方法。这并不能解决问题——基板还包括双接头来分离所有的引脚——但是以太网、串行和 SD 肯定减少了添加所有这些的需要。硬件的另一个缺点是示例固件是针对 IAR 嵌入式工作台的，它既不是免费的，也不是业余爱好者可以负担得起的。

基板上使用的网卡具有自动交叉功能，因此这些板使用常规的 Cat6 跳线连接。本例中，电路板不断发送 UDP 数据包，右侧的模块通过串行连接向终端报告状态信息。