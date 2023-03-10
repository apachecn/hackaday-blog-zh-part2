# 用机械臂测量磁场

> 原文：<https://hackaday.com/2014/03/30/measuring-magnetic-fields-with-a-robotic-arm/>

![MagneticArm](img/3866467c06746bb5c5f141ef4750b2c5.png)

学习磁铁和磁场的工作原理是一回事，但实际上能够测量和观察磁场完全是另一回事！[Stanley]的最新项目使用了一个连接到具有 3 个自由度的机械臂上的[磁力计来测量磁场。](http://www.stanleylio.com/home/magnetic-field-measurement)

使用从易贝购买的伺服系统和铝制安装硬件，[Stanley]建造了一个简单的机器人手臂。然后，他将一个 HMC5883L 磁力计挂在机械臂上。[Stanley]使用 Atmega32u4 和 [LUFA](http://www.fourwalledcubicle.com/LUFA.php) USB 库与该传感器接口，因为它具有高数据速率。对于那些不熟悉 LUFA 的人来说，它是一个用于 AVRs 的轻量级 USB 框架(以前称为 MyUSB)。结果是在 MATLAB 中绘制的( [Octave](https://www.gnu.org/software/octave/) 是免费的 MATLAB 替代品)，这是一种非常强大的基于数学的脚本语言。这些图几乎完全符合在磁学入门课上学到的磁场模式。休息后一定要看视频中的机器人手臂进行测量，这非常酷！

[Stanley]在他的文章末尾慷慨地为他的项目提供了 AVR 代码和 MATLAB 脚本。这将是非常酷的，看看还有什么传感器可以用这种方式！还有什么其他的自然现象在三维地图上会很有趣？

[https://www.youtube.com/embed/YU3vraleH0I?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&start=31&wmode=transparent](https://www.youtube.com/embed/YU3vraleH0I?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&start=31&wmode=transparent)