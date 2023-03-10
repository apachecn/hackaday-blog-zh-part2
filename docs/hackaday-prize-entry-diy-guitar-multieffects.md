# Hackaday 奖参赛作品:DIY 吉他多重效果

> 原文：<https://hackaday.com/2015/08/08/hackaday-prize-entry-diy-guitar-multieffects/>

吉他效果和其他音乐电路是对电子学的一个很好的介绍。这是有原因的:对于音频电路，你处理的是模拟信号，而不仅仅是 LED 闪烁的 1 和 0。再加上音频效果的 DSP 方面，你就可以在一个项目中完成几门电子工程学位课程。

为了他的 Hackaday 奖参赛作品，[randy.day]正在制作一个多效吉他。这个小小的 PCB 不仅仅是一个失真、模糊或合唱电路，它还将具有几种音调变换的味道，侧翼、合唱、回声、和声以及更奇怪的“数字化”效果，如比特粉碎。

这个效果单元是围绕 PIC32 和一个以 64k 32 位采样/秒处理音频的 [TI 音频编解码器](http://www.ti.com/product/tlv320aic3204)构建的。这负责所有的音频处理，但吉他踏板的艰苦工作实际上是外壳和机械——这是舞台设备的艰苦生活。对于脚踏板输入，[兰迪]正在使用一个磁性位置传感器，但没有消息表明他是否会使用一个花哨的压铸外壳或塑料注射成型单元。

#### 2015 年[黑客日奖](http://hackaday.io/prize)由以下机构赞助:

[![](img/8e6c49d55ea91b307d7d191b75ab18c8.png)](http://hackaday.io/atmel)[![](img/6b53a13e67e0346985e237ef126c1bcc.png)](http://hackaday.io/freescale)[![](img/3fe105965ef22414d89f71032d9babee.png)](http://hackaday.io/microchip)[![](img/ebcbe4e97993de26ebcf849e70523a14.png)](http://hackaday.io/mouser)[![](img/15f4f8aaed16b020832d8be6282e47f5.png)](http://hackaday.io/ti)