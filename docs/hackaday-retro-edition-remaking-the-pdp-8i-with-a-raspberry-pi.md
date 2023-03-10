# Hackaday 复古版:用树莓 Pi 重新制作 PDP 8/I

> 原文：<https://hackaday.com/2015/03/26/hackaday-retro-edition-remaking-the-pdp-8i-with-a-raspberry-pi/>

[Oscar]非常喜欢 PDP-8s，极其老派的 PDP-8/I 是他的最爱。如果你最近没有检查过这些的价格，得到一个真正的 PDP-8/I 几乎是不可能的。然而，在组装了 KIM-1 克隆工具包后，一个想法出现了:建造一个现代 PDP-8/I 复制品怎么样，它看起来像真的一样，但由现代硬件驱动。这将是相当便宜的建设，并有额外的好处，没有几百磅重。

[PiDP-8 是[Oscar]的项目](http://hackaday.io/project/4434-pidp-8i),以现代形式复制 8/I 的硬件。代替数百个倒装芯片，这个 PDP-8 由运行[SIMH 仿真器](http://simh.trailing-edge.com/)的树莓 Pi 驱动。Pi 上的 40 针 GPIO 连接器被分解成一个大 PCB 上的 92 个 led 和 26 个拨动开关。这个设置给了[Oscar]一个合理的 PDP-8/I 的复制品，但是他也选择了*的外观*。[他制作了一个丙烯酸面板](http://hackaday.io/project/4434-pidp-8i/log/14646-acrylic-panel-sent-off)，其插图是从安装在 PCB 上的原始 8/I 复制而来的，使整个项目呈现出 60 年代末/70 年代初美丽的棕色，并带有丰收金色的色彩。

由于这种模拟的 PDP-8/I 运行在全新的硬件上，因此携带像小孩一样大的磁盘驱动器、磁带驱动器和纸带阅读器没有多大意义。相反，[奥斯卡]把所有东西都放在 u 盘上。对于移动几千字大小的文件来说，这是一个很好的解决方案。

![vt100normal](img/feb3dafab4e4c1a5d2af53414a3bdeb2.png)【Oscar】说他将带着他的 PiDP 参加 4 月 17 日至 19 日在新泽西州沃尔举行的[老式电脑节东 X](http://www.vintage.org/2015/east/) 。我们会去的，我已经让[奥斯卡]使用 VT-100 终端。如果你在这个地区，*你应该来参加这个活动*。这肯定会是一个令人敬畏的事件，你一定会玩得很开心。由于这是 PDP-8 推出 50 周年，将有半打原始 PDP-8 成立，包括一个新翻新的直-8 来自[电阻](http://makerspace.rutgers.edu/content/tribute-resistors)。

哦，如果有人知道如何将 Pi 连接到 VT100(技术上是 103)，请在评论中留言。它需要 RTS/CTS 吗？