# ESP8266 密切关注您的电池

> 原文：<https://hackaday.com/2015/05/24/esp8266-keeps-and-eye-on-your-batteries/>

关于电池，除了在任何给定时刻的电压和电流输出之外，还有很多东西需要了解，其中大多数无法用标准万用表测量，除非你也拿着 Excel 电子表格站在那里很长时间。最有用的信息是电池容量，它可以告诉你电池充满电或完全放电还剩多少时间。[TJ]着手创建电池数据采集器，[使用无处不在的 ESP8266 制作全功能电池监控器](http://www.esp8266-projects.com/2015/05/battery-live-monitor-system-esp8266.html)。

测量电池容量非常简单，但需要时间。首先对电池进行基准测试，以确定其理想容量，然后可以读取未来的电压和电流读数，并与基准测试进行比较，以确定电池的当前容量。ESP8266 是这类工作的相对较好的选择。它的 WiFi 连接允许它向服务器报告信息，服务器将存储数据并让用户可以看到。

这个项目的第一页详细介绍了实际模块的构建，第二页概述了如何让模块与服务器通信。一旦你完成了这一切，你就可以用它来监控你的[全屋 UPS 备份系统](http://hackaday.com/2012/04/09/ups-with-dead-batteries-reborn-as-a-whole-house-power-backup/)或者你的太阳能卡车中的[电池。在项目网站上有相当多的信息可以用来重新构建你自己，下面还有一个视频展示了它的操作。](http://hackaday.com/2012/05/16/prototyping-a-solar-charger-for-your-truck/)

[https://www.youtube.com/embed/mIq-dujJ_Yo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/mIq-dujJ_Yo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)