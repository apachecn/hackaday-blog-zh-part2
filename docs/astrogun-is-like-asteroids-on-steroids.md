# ASTROGUN 就像类固醇上的小行星

> 原文：<https://hackaday.com/2014/07/27/astrogun-is-like-asteroids-on-steroids/>

![Astrogun](img/492d64b856570ffc4379adc323169a47.png)

随着耶路撒冷迷你 Makerfaire 的到来，[Avishay]不得不拿出一些东西来建造。他的最后一个项目是他称之为 ASTROGUN 的东西。ASTROGUN 是一种增强现实游戏，玩家试图在被击中之前快速接近小行星。

这绝对让人想起街机经典，小行星。主要的区别是玩家没有太空船，也不在太空中移动。相反，玩家拥有第一人称视角，可以 360 度旋转并上下观看。角落里的雷达屏幕会让你大致了解小行星来自哪里。然后就看你的了，在他们摧毁你之前，找到他们，并把他们炸得灰飞烟灭。

这个游戏是围绕着一台树莓派电脑构建的。这充当了操作的大脑。Pi 与一个 [MPU-9150](http://www.invensense.com/mems/gyro/mpu9150.html "MPU9150") 惯性测量单元(IMU)接口。你通常会在无人机上看到 IMU 来帮助它们保持方向。在这种情况下，[Avishay]用它来跟踪爆破工的运动和方向。他声称这个装置有九个自由度。

Pi 生成图形，并将输出发送到一个小的高亮度 LCD 屏幕。屏幕垂直于玩家的视线安装，因此屏幕朝上。有一小块分束玻璃以大约 45 度角安装在显示器上方。这是一种特殊的玻璃，部分反射，部分半透明。结果是玩家透过玻璃看到真实世界的背景，数字图形覆盖在其上。类似于一些平视显示技术。

所有的电子设备要么安装在玩具枪内部，要么安装在玩具枪周围。展示系统附有一个定制的玻璃纤维底座。代码似乎可以通过 [Github](https://github.com/avishorp/astrogun "Github") 获得。请务必观看下面的系统运行视频。

[https://www.youtube.com/embed/QMrVHVkC-Qw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/QMrVHVkC-Qw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[通过 T0 黑客攻击。io]t1