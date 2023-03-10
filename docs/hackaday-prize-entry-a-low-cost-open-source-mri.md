# Hackaday 奖参赛作品:低成本、开源 MRI

> 原文：<https://hackaday.com/2015/05/04/hackaday-prize-entry-a-low-cost-open-source-mri/>

[这种低成本磁共振成像器](https://hackaday.io/project/5030-low-field-mri)并不是【Peter】第一次尝试医学成像，也不是他第一次参与 Hackaday 奖的项目。[他已经使用钡检查源和作为高能粒子探测器销售的 CCD 建造了一台 CT 扫描仪。他去年的 Hackaday 奖参赛作品，](http://hackaday.com/2013/10/23/towards-a-low-cost-desktop-ct-scanner/)[开源科学三录仪](https://hackaday.io/project/1395-open-source-science-tricorder)的传感器足以让【斯波克】嫉妒，[最终获得第四名](http://hackaday.com/2014/11/13/satnogs-wins-the-2014-hackaday-prize/)。

[Peter]的 MRI 扫描仪解决了他的开源 CT 扫描仪的一些缺点。虽然 CT 扫描仪工作正常，但它非常慢，需要几个小时才能对一个柿子椒成像。这主要是由于他的粒子探测器的灵敏度和他所能获得的检查源的温度。与高放射性元素不同，你可以*制造*高强度磁场，这使得这种 MRI 扫描仪可能比 CT 扫描仪有用得多。

有几件事使得低成本的 MRI 机器成为可能，首先是一种可视化磁场的方法。为此，[Peter]使用了 Honeywell HMC5883L 三轴磁力计阵列，这是他能找到的最小的传感器，但范围最大。这些磁强计是 I2C 器件，所以用几个多路复用器，它实际上是一个相对简单的构建。

用这些磁力计成像并不简单，要从这台磁力相机看到的所有噪音中产生一个信号需要做大量的工作。[Peter]将使用的技术与 2014 年 Hackaday 奖的另一个参赛项目[质子旋进磁力计](http://hackaday.io/project/1376-pyppm-a-proton-precession-magnetometer-for-all)没有太大区别。当你身体中的质子暴露在高强度磁场中时，它会朝向高强度磁场。当大磁场关闭时，质子会将自己朝向下一个最强的磁场，在这种情况下，就是地球。当质子朝向地球磁场时，它会轻微振荡，这种衰减振荡正是磁相机实际检测到的。

利用[Peter]的出版物中的一些技术[，这些振动可以变成图像。它的分辨率不会和装满整个房间的核磁共振成像仪一样高，但是它可以工作。想象一下，一台由激光切割胶合板制成的核磁共振成像设备将放在桌面上。没有比这更酷的项目了。](http://spie.org/Publications/Proceedings/Paper/10.1117/12.918856)

* * *

#### 2015 年[黑客日奖](http://hackaday.io/prize)由以下机构赞助:

[![](img/8e6c49d55ea91b307d7d191b75ab18c8.png)](http://hackaday.io/atmel)[![](img/6b53a13e67e0346985e237ef126c1bcc.png)](http://hackaday.io/freescale)[![](img/3fe105965ef22414d89f71032d9babee.png)](http://hackaday.io/microchip)[![](img/ebcbe4e97993de26ebcf849e70523a14.png)](http://hackaday.io/mouser)[![](img/15f4f8aaed16b020832d8be6282e47f5.png)](http://hackaday.io/ti)