# 一种用于逆向计算机的过杀网络适配器

> 原文：<https://hackaday.com/2013/05/28/an-overkill-network-adapter-for-retrocomputers/>

![amiga](img/369c74b22629f417eff7573b7dbbd6b3.png)

如果你想在网上买一台旧的苹果电脑、64 代康茂德电脑、阿米加电脑或任何其他的翻新电脑，这是给你的。[Stian]有一台 Amiga 500，想放在网络上。A500 是不可扩展的，所以他需要寻找某种适配器来把它放到网络上。他找到了解决方案，一个树莓派、一根零调制解调器电缆和一些软件。

为了将他的 Amiga 连接到网络，[Stian]为他的 Raspi 制作了一个小型串行转换器板，将 pi 上的 Tx 和 Rx 引脚连接到一个 9 引脚串行端口。与 Pi 的物理连接完成后，剩下唯一要做的事情就是为 Amiga 获取一些软件，即 [AmiTCP](http://aminet.net/package/comm/tcp/AmiTCP-demo-40) 和 [PPP](http://aminet.net/package/comm/net/PPP1_45) 。这不完全是一个*快速*网络连接，但这种构建允许【Stian】用古老的硬件连接到 WiFi 网络。

[Stian]构建的一个有趣的方面是，它完全可以转移到其他复古计算机上——从旧的 S-100 总线计算机到经典的 MAC、apples，以及几乎任何其他具有支持 PPP 的串行端口的计算机。即使有树莓 Pi 的费用，它也比贵得离谱的二手 SCSI 到以太网控制器和其他愚蠢的东西便宜得多。