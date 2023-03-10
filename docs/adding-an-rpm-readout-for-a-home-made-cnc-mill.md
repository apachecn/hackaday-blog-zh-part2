# 为国产数控铣床增加转速读数

> 原文：<https://hackaday.com/2014/02/08/adding-an-rpm-readout-for-a-home-made-cnc-mill/>

![rpm_lcd](img/30e348f2d75531c1e533a48498c3c04b.png)

[Rui]最近对他自制的数控铣床进行了最后的加工，该铣床使用了一种类似 dremel 的旋转刀具。在这种应用中使用旋转工具的问题是你没有准确的速度读数…所以他设计了自己的转速计。

传感器本身非常简单。他使用了一个 TLE4935L 霍尔效应传感器、一个备用的 16FE88 微控制器、一个诺基亚 LCD 和一个微小的钕磁铁。磁铁被小心地用环氧树脂粘在电机风扇上，霍尔效应传感器就在旁边。他还在它周围建立了一个防护装置，以防磁铁决定高速飞离。

在测试过程中，他将霍尔效应传感器连接到自制的电路和示波器上，以证实他的发现。一旦他确信一切正常，他就把它封起来，并把 LCD 安装在主轴上方，作为一个漂亮的数字读数器。

[https://www.youtube.com/embed/UTgcLeo4SlI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/UTgcLeo4SlI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

这也不是芮第一次为头版增色了——他还制作了一个伟大的[激光测距仪黑客](http://hackaday.com/2011/10/10/ultrasonic-rangefinder-as-scanning-radar/)和[气枪游戏的激光绊线！](http://hackaday.com/2011/09/11/laser-trip-wire-in-an-easy-to-use-form-factor/)