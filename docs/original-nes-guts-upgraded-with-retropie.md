# 原始 NES 内脏升级为 RetroPie

> 原文：<https://hackaday.com/2014/06/01/original-nes-guts-upgraded-with-retropie/>

如果你有一辆破旧的 NES，却不知道如何处理它，你可能想看看[SnO ius]的最新项目。他用覆盆子酱取代了他的老 NES 的内脏。[snoius]首先从他原来的 NES 上拆下大部分电子设备，为 Pi 腾出空间。他留下了原来的控制面板，以便能够使用原来的电源按钮和电源指示灯。NES 电源开关是一个开/关拨动开关。[snoius]决定将 5V USB 电源输入直接通过该开关。其结果是微型计算机的硬电源开关。原来的电源 LED 通过一个 330 欧姆的电阻连接到 Pi 的 3.3V GPIO 头。现在，当 Pi 通电时，LED 会亮起。

下一步是控制器。看起来像[snoius]正在使用一些 USB SNES 控制器克隆。他想使用原来的 NES 控制器端口，但显然 NES 没有利用 USB。[snoius]用锯子锯掉控制器端口的背面，留下一个平坦的表面。然后，他用一把美工刀在一个母 USB 接口的形状上挖了一个洞。他在适当的位置安装了一些端口，然后用电线将内部连接到一些带有公头的短 USB 电缆上。这些插头插入了隐藏在 NES 盒子里的 USB 集线器。

Pi 还连接到一根短 HDMI 电缆和一根短电源线。电缆的松散端安装在一个小木块上。木头上切出缺口，以便更好地配合电缆末端。NES 的后部在原来连接器的位置切出两个孔，以容纳新的连接器。

尽管所有的硬件都考虑到了，snoius 仍然需要一种方法来玩他的游戏。这就是 [RetroPie](http://blog.petrockblock.com/retropie/ "RetroPie") 拯救世界的地方。RetroPie 是一个针对 Raspberry Pi 的 Linux 发行版，它是专门为使玩旧视频游戏变得容易而创建的。它包括许多老系统的模拟器，包括 NES，SNES，SEGA 创世纪，Gameboy 等。[snoius]把 RetroPie 安装到 8GB 的 SD 卡上，复制了他能找到的所有 rom。最终的结果是什么似乎是一个原始的 NES 一眼，但实际上是多个复古游戏系统在一个。它还在板载内存中包含数百个视频游戏，而不需要大型物理盒式磁带库。

[via [reddit](http://www.reddit.com/r/raspberry_pi/comments/26swo2/completed_retropie_build_in_an_nes/ "Reddit.com")