# 连接您的家庭安全系统

> 原文：<https://hackaday.com/2012/07/30/getting-connected-with-your-home-security-system/>

![](img/a1447d6890d8935a5e739aae6be71b2c.png "wireless-link-for-home-security-system")

这个简单的设备，配以一些创建代码，将让你[成为你自己的家庭安全监控服务](http://www.phantomlink.com/diy.aspx)。它被称为 PhantomLink，亚当将这个项目作为一个商业项目启动。他最近决定对硬件进行开源，并将很快发布一个关于如何编写自己的 web 界面的指南。

我们刚刚关注了一个项目，该项目使用 Arduino 来控制安全面板。PhantomLink 不仅关注输入硬件的重用，还关注整个系统的监控。听起来好像支持几种不同的协议。

DB9 插孔旨在与您可以自己接线的适配器一起使用。基本上只需接入你家报警控制器上的端子板，然后将这些连接路由到适当的引脚。PIC 12F683 监控报警系统，通过安装在板上的 WiFi 模块推送数据。有了这个网络连接，你可以通过捕捉和格式化数据来做任何你想做的事情。