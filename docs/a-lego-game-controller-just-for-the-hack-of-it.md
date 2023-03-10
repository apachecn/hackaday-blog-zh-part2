# 一个乐高游戏控制器；只是为了好玩

> 原文：<https://hackaday.com/2014/07/30/a-lego-game-controller-just-for-the-hack-of-it/>

![ExwDPUV](img/837bf24976867d1069fae0d55b6f5fa4.png)

[StrangeMeadowlark]有一天决定创造出[这款基于 Arduino 的游戏控制器](http://strangemeadowlarkprojects.blogspot.com/2014/05/a-legoarduino-game-controller.html)。没有任何特别的原因，除了，为什么不呢？！

它看起来像一艘从附近星球飞来的小型乐高宇宙飞船，直接飞向一个渴望的地球玩家手中。通过银色的按钮，这个设备可以玩传送门 1 和 2，加里的 Mod，《我的世界》和 VisualBoy Advance。虽然还需要做更多的工作，但是控制器完成了这项工作；尤其是玩口袋妖怪的时候。感觉像 Gameboy 界面，有可定制的外框。

粘性的蓝色大头针固定住几根电线。而且，大多数材料都是在房子周围找到的。比如上面的游戏手柄按钮；它们是普通的触觉开关，可以从简单的电子设备中提取出来。还有乐高，它提供了一种简单的方式来建造车身控制台，而不是去找 3D 打印机和学习 AutoCAD。

![ssf3wKS](img/b4765f8a1d33a505fce07a674ecaf23a.png)

PC 和 Arduino 内部的通信是通过让控制器假装成 USB 键盘来完成的，允许游戏中的按键映射。按键被发送到固件专用缓冲区中的串行转 USB 芯片。更不用说，如果有需要，它还提供了浏览 Imgur 的选项。

对于未来的迭代，可能会添加操纵杆。将它们集成到控制器中需要一些时间，但这是值得的。另一个实现将是利用游戏手柄固件来代替模拟键盘，后者不报告模拟值。

其他类似的乐高项目还有这个[两轴平移延时装置](http://hackaday.com/2011/08/12/two-axis-panning-time-lapse-rig-built-from-lego/)，这个[定制的电子乐高微控制器系统](http://hackaday.com/2013/07/05/legoduino-for-kid-friendly-microcontrollers/)叫做 LegoDuino，这个避障[带 CD 轮的乐高漫游车](http://hackaday.com/2013/09/01/obstacle-avoiding-lego-rover-uses-cds-for-wheels/)，这个[乐高绘图机](http://hackaday.com/2014/07/13/lego-drawing-machine-draws-block-shapes-best/)，还有这个 [DIY 分光光度计](http://hackaday.com/2011/05/20/diy-spectrophotometer/)。