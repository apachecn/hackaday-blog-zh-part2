# 使用 Arduino Shields 搭配树莓 Pi

> 原文：<https://hackaday.com/2012/05/06/using-arduino-shields-with-the-raspberry-pi/>

![](img/51d2adb1bfa4efb0b947e8dc86e1ca33.png "ponte-layout-revc")

自从 Arduino 几年前推出以来，已经发布了许多提供附加功能的“屏蔽”或附加板。有数百种不同的屏蔽，从视频捕捉屏蔽到触摸屏屏蔽。现在树莓皮已经在野外了，树莓皮到阿杜伊诺的屏蔽桥(T1)的建立只是时间问题。

[Omer]称他的桥为“Ponte ”,它允许 Arduino shields 以嵌入式 Linux 系统难以置信的马力使用。虽然[Omer]最初期望自己编写 RasPi 到 Arduino 软件转换器，但是在构建中途发现了 [WiringPi](https://projects.drogon.net/raspberry-pi/wiringpi/) 。当然，这个版本是在我们看到关于[控制 RasPi](http://hackaday.com/2012/05/05/controlling-raspberry-pi-expansion-pins-with-a-web-interface/) 上的 GPIO 管脚的教程后一天发布的，我们希望在未来看到类似的 GPIO 黑客版本。

目前，Ponte 只支持 Arduino Uno 大小的盾牌，因此使用 [RAMPS](http://reprap.org/wiki/Arduino_Mega_Pololu_Shield) 电机驱动器的一体化 RepRap 控制器的可能性目前是不可能的。我们希望随着越来越多的人收到他们的拉斯皮，这种情况会很快改变 T2。