# 电动小鬼让猫门鸣叫它的活动

> 原文：<https://hackaday.com/2013/01/04/electric-imp-makes-a-cat-door-tweet-its-activities/>

![electric-imp-tweeting-cat-door](img/d053d3f77a6932704399bb8d5789353e.png)

这个 [Tweeting 猫门使用电动 Imp](http://whiskeytangohotel.com/ourcatdoor) 来读取传感器并向服务器报告。硬件相当整洁。该主板搭载 ARM Cortex-M3 处理器，并通过 WiFi 接入您的家庭网络。迷你 USB 电缆只是提供电源。编程是通过网络完成的。我们自己的[【布莱恩·本考夫】在秋天早些时候有机会试用小恶魔](http://hackaday.com/2012/09/04/hands-on-with-the-electric-imp/)。

监视猫门是承担一个项目的最好理由。添加到板上的硬件包括安装在门框上的簧片开关以及门上的磁铁。还有一个蓝色的 LED，可以提供一点用户反馈。这个软件不太容易，但也没那么糟糕。与大多数网络连接项目一样，让所有部分相互通信有点麻烦。Imp 向本地网络上的服务器报告，然后服务器激活一个 PHP 脚本，该脚本使用 [Sen.se](http://open.sen.se/) 发送推文。

[谢谢帕特]