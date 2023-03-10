# 超音速 NERF 飞镖速度计

> 原文：<https://hackaday.com/2014/08/03/supersonic-nerf-dart-speedometer/>

![ATtiny Chronograph](img/43871d8ac378364f3da7bde67afbf0c6.png)

[约翰]面临着一个有趣的问题:在他建造了自己的空气炮后，他如何准确地说出他的 NERF 飞镖移动的速度？幸运的是，他手头有一些备用零件，用比 Arduino 还低的价格拼凑了一个[全功能抛射速度表](http://www.instructables.com/id/Attiny-projectile-speedometer/)。

一个设备实际上是两个彼此相隔精确距离的检测器。当物体通过第一个探测器时，一个计时器被激活，测量物体到达第二个探测器需要多长时间。由此，设备计算速度。[John]使用间隔正好为 3 英寸的红外发射器/探测器对，并将它们连接到 ATtiny2313。经过一点点编码，他现在知道他能以多快的速度发射那些粘糊糊的弹道导弹。

红外发射器/探测器对安装在投射物穿过的 PVC 管上。[John]指出，从理论上讲，这可以用来测量几乎任何可以通过管道的东西，尽管这种特殊的设备可能会被枪口闪光或实际枪支的压力波损坏。

在之前，我们已经看过了[其他的 NERF 飞镖空气炮，我们想知道是否应该进行某种比赛，看看谁能最快地射出 NERF 飞镖，现在有一种简单的方法来测量速度了？](http://hackaday.com/2012/09/18/how-to-build-an-extremely-powerful-nerf-gun/)