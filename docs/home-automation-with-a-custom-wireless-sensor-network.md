# 具有定制无线传感器网络的家庭自动化

> 原文：<https://hackaday.com/2014/10/11/home-automation-with-a-custom-wireless-sensor-network/>

我们对这里的家庭自动化项目并不陌生，但你很少能看到如此详细的描述。[Paul]与四名队友为一个本科论文项目设计了一个[定制家庭自动化系统](http://pbooleanprojects.blogspot.ca/2014/09/arduimu-based-home-automation-system.html "custom home automation system")。

该系统分为两个主要部分:服务器和外围设备。该团队根据即将推出的 ArduIMU v4 测量单元的早期原型设计了他们的外设。他们移除了所有默认传感器，以降低成本并减少组装时间。这些装置可以连接到各种外围设备，如温度传感器、电源继电器、RGB 色带等。

使用基于网络的用户界面对系统进行集中管理。web 服务器运行在 Java 上，通过无线方式与外围设备交互。基本消息可以来回发送，以读取外设的状态或改变状态。就用户而言，这些消息显示为简单的触发器和动作。这使得使用 if，then，else 逻辑对外设进行编程变得非常简单。

主项目页面是一个非常简短的摘要，它似乎是一个文档非常完整的项目。该团队已经公开了他们的 [182 页的最终报告](http://ece.eng.umanitoba.ca/undergraduate/ECE4600/ECE4600_Files/Archive/2013/2013_2014_Final_Reports/G07_Final_Report_2014.pdf "final report") (pdf)，该报告深入了该项目的本质细节。另外，一定要看下面的演示视频。

[https://www.youtube.com/embed/xdKUvubAaFM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/xdKUvubAaFM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)