# 自动捡拾绕线机

> 原文：<https://hackaday.com/2014/05/24/the-automated-pickup-winding-machine/>

当电吉他还是一个新事物的时候，缠绕拾音器是一个非常耗费人力且容易出错的过程。几百圈的导线很容易改变线圈的数量，使得最终的拾音器要么贫血，要么比吉他中的其他拾音器强大得多。[Davide]开始给自己的拾音器上弦，希望比简单猜测一个线圈有多少圈更精确一点[他造了一个 AVR 线圈绕线机](http://davidegironi.blogspot.it/2014/05/a-pickup-winding-machine-built-on.html)。

该机器使用转速为 1200 转/分的 DC 齿轮马达。磁铁粘在电机轴上，连接到 ATMega8 的霍尔效应传感器跟踪线圈上有多少绕组。

界面简单，使用字符液晶显示一个风计数器，电机方向，和当前电机速度。这台机器有一些有用的功能:慢速启动和自动停止使缠绕皮卡比用缝纫机缠绕皮卡的传统家庭方法容易得多。

[https://www.youtube.com/embed/gNgywx7ITok?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/gNgywx7ITok?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)