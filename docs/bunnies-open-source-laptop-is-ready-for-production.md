# [Bunnie]的开源笔记本电脑已经可以生产了

> 原文：<https://hackaday.com/2014/01/12/bunnies-open-source-laptop-is-ready-for-production/>

就在一年前，[Bunnie Huang]宣布他正在进行一个非常雄心勃勃的个人项目:[一款完全开源的笔记本电脑](http://hackaday.com/2012/12/16/bunnie-builds-a-laptop-for-himself-hopefully-us/)。现在，在他的硬件黑客同胞[xobs]的帮助下，这台名为[no vena 的笔记本电脑接近完成。](http://www.bunniestudios.com/blog/?p=3597)

在着手这个项目之前，[Bunnie]对设计有一些必备的要求。最重要的是，所有的组成部分应该是免费的 NDA 产权负担。这不是一项容易的任务；将文档放在服务器上的 SoC 供应商少之又少，而飞思卡尔是唯一符合要求的供应商。其次，整个笔记本电脑应该是完全开源的。[Bunnie]找不到开源 GPU，所以在他的笔记本电脑上使用硬件视频解码需要二进制 blob。不过，软件解码工作得很好。

此外，这款笔记本电脑设计用于安全和硬件入侵。两个以太网端口(一个 1gb，另一个 100Mbit)，一个 USB OTG 端口和一个 Spartan 6 FPGA 使这台笔记本电脑自成一类。主板包括 8 个模拟输入、8 个数字 I/O 端口、8 个 PWM 引脚和一个 Raspberry Pi 兼容接头，用于一些真正的硬件黑客。

至于笔记本电脑的规格，对于高端平板电脑来说，它们是值得尊敬的。CPU 为飞思卡尔 iMX6，四核 ARM Cortex-A9，主频 1.2 GHz。RAM 可升级到 4GB，内部 SATA-II 端口将轻松容纳一个巨大的 SSD，使用 LCD 适配器板运行 13 英寸 2560×1700 LED 面板的能力[Bunnie]正在使用。电力系统旨在模块化，电池由普通的 RC Lipo packs 提供。欲了解完整的规格，请查看维基。

尽管[Bunnie]的笔记本电脑价格较高，性能相对较低(与 i7 笔记本电脑相比)，但人们对旋转几千块电路板并将其发送出去进行挑选和放置很感兴趣。在 2 月下旬或 3 月的某个时候，将会有一场围绕“带电池的一体式 PC”外形的 Novena 众筹活动。没有确切的数字表明诺维娜的价格，但不言而喻的是，不管怎样，它都会卖出很多。

如果你想要最新的更新，最好去官方的 Novena Twitter:[@ novenakosagi](https://twitter.com/intent/user?screen_name=novenakosagi)