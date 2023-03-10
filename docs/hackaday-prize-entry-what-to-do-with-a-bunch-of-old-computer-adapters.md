# 黑客日奖参赛作品:如何处理一堆旧电脑适配器

> 原文：<https://hackaday.com/2015/07/02/hackaday-prize-entry-what-to-do-with-a-bunch-of-old-computer-adapters/>

回到 2014 年 Radio Shack 还存在的时候，你可以开车到美国的任何一个购物中心，购买早在 1972 年就生产的 D-sub 连接器。是的，你能在旧电脑上找到的所有那些 SCSI、串行、并行和其他奇怪端口的连接器不到五美元就能买到。出于这样或那样的原因，[yesnoio]有很多这样的连接器。不仅仅是连接器，还有那些夹在连接器上的小塑料壳。如何处置他们？[复古模块](https://hackaday.io/project/5722-retro-modules)！基本上就是 littleBits 如果 littleBits 是 1987 年发明的。

复古模块的目标是能够将原型放入你的背包中，而不需要从试验板上扯下一两根电线。基本的基础是要有一个规范，概述 DB-25 和 DE-9 连接器的引脚排列，将这些信号用于电源、ic 总线。模拟线路和 SPI 线路。将一个微控制器放在一个塑料壳里，将一个传感器放在另一个里，将一个显示器放在第三个里；你有一个电子原型平台，它是在一个无线电室的密室里设计的。

[yesnoio]有[入门指南](https://github.com/makerblueprint/retrospecification)，带你完成前三个复古模块的创建。第一个是一个 Arduino nano 或 micro，塞在一个塑料外壳中，带有一个 DA-15 母连接器。第二个模块只是一个 LED 和电阻，第三个只是一个伺服。这些可以连接在一起，并且由于规范的原因可以控制。它很聪明，有点疯狂，而且有可能比你在 Maker Faire 上找到的任何电子原型平台都要酷得多。

#### 2015 年[黑客日奖](http://hackaday.io/prize)由以下机构赞助:

[![](img/8e6c49d55ea91b307d7d191b75ab18c8.png)](http://hackaday.io/atmel)[![](img/6b53a13e67e0346985e237ef126c1bcc.png)](http://hackaday.io/freescale)[![](img/3fe105965ef22414d89f71032d9babee.png)](http://hackaday.io/microchip)[![](img/ebcbe4e97993de26ebcf849e70523a14.png)](http://hackaday.io/mouser)[![](img/15f4f8aaed16b020832d8be6282e47f5.png)](http://hackaday.io/ti)