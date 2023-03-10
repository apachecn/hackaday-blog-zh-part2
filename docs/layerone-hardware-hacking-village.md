# LayerOne 硬件黑客村

> 原文：<https://hackaday.com/2015/05/24/layerone-hardware-hacking-village/>

去 DEFCON，你会排五个小时的队，得到一个花哨的电子徽章，有一天你会展示给你的孙子。是的，在 DEFCON，你买你的黑客信誉。LayerOne 对技术不熟练的人不太友好。在 LayerOne，你会得到一个 PCB，一袋零件，并被告知通过手工焊接微小的 QFP 和 SOT-23 芯片来获得黑客信誉。LayerOne 的硬件黑客村挤满了急切组装徽章的人，或者根据他们有多酷来组装徽章。

徽章是由零空间实验室的[查理 x]设计的，零空间实验室是该地区众多本地黑客空间之一。这些徽章的设计和构造记录在 hackaday.io 的 LayerOne 徽章项目中，它们可能是我们见过的最好的诈骗徽章。

有两个徽章分布在 LayerOne 周围。第一个是一个非常亮眼的徽章，由 Cypress PSoC4 控制 22 个可单独寻址的 RGB LEDs。大多数与会者都会收到一个裸露的 PCB 和一袋零件——PCB 会让你进门，但如果你想要你的书呆子信誉，你必须自己组装徽章。

这个徽章仍然有一些有趣的功能，包括一个 ESP8266 模块，它将侦听 UDP 数据包并驱动 led。是的，同一个 WiFi AP 上的一个随机的人可以控制整个会议活动的 led。徽章也可以用三根电线连接在一起，但迄今为止还没有人做到这一点。

[![vocore](img/717bb29a35d350461f803a9c3c7832a4.png)](https://hackaday.com/wp-content/uploads/2015/05/vocore.jpg)

The Speaker and Staff badge, based on a VoCore

第二个徽章——针对演讲者和工作人员——格外强大。它是一个徽章上的 Linux 盒子，带有两个运行 OpenWRT 的以太网连接器。对于一个 con 徽章来说，它非常强大，但这不是 LayerOne 会议上计算最复杂的徽章。对于去年的徽章，[charlie]用 FPGA、SAM7 微控制器、SD 卡和有机发光二极管显示器组装了一个徽章。他们在这些徽章上挖矿。

硬件黑客村装载了十几个金属烙铁、双目显微镜和足够的焊料、灯芯和助焊剂，让每个人都能把他们的徽章焊接在一起。每个尝试过的人实际上都完成了他们的徽章，其他骗局中徽章黑客竞赛的故事充满了人们在随机焊盘上撒元件的故事。想象一下:在一个会议上，人们都是技术专家。太神奇了。

 [![A hot plate was available for those who were not cool enough to solder 22 smd LEDs](img/4a0f9bbdba5bd0a6c73e1f863643e73b.png "plate")](https://i0.wp.com/hackaday.com/wp-content/uploads/2015/05/plate.jpg?ssl=1) A hot plate was available for those who were not cool enough to solder 22 smd LEDs [![awesome hat](img/dcb9fa65f456f223006a3017cc63471b.png "awesome hat")](https://i0.wp.com/hackaday.com/wp-content/uploads/2015/05/awesome-hat.jpg?ssl=1)  [![microscope](img/80f7069fd879bc82da4bc0fae2a39b49.png "microscope")](https://i0.wp.com/hackaday.com/wp-content/uploads/2015/05/microscope.jpg?ssl=1)  [![SMD solder stencil for the LEDs](img/2090047377f81b6222867251956b76cc.png "stencil")](https://i0.wp.com/hackaday.com/wp-content/uploads/2015/05/stencil.jpg?ssl=1) SMD solder stencil for the LEDs