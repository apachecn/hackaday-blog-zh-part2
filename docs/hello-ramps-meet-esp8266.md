# 你好，斜道，见见 ESP8266

> 原文：<https://hackaday.com/2015/08/20/hello-ramps-meet-esp8266/>

DIY 3D 打印机的激增在很大程度上得益于令人敬畏的开源 RepRap 项目。这个项目的一个主要部分是斜坡板——一个单独的控制板/护罩，打印机的所有其他部分都可以很容易地连接到它上面。USB 连接到计算机是通常的选择，除非 RAMPS 板有 SD 卡选项，允许 3D 打印机不受限制地运行。CreatorBot 的[Chetan Patil]制作了一个[分线板，帮助将 ESP8266 WiFi 或 HC-05 蓝牙模块连接到斜坡板上的 Aux-1 接头](http://creatorbot.com/projects/electronics/add-esp8266-wifi-to-your-3d-printer)。这使他能够将 g 代码流式传输到打印机，并允许远程控制和监控。

虽然廉价的 ESP8266 模块是黑客们的当季流行，但让它们工作起来可能是一件非常令人头疼的事情。所以[Chetan]做了一些黑客工作来找出在 ESP 模块上开发的工具链，并发现 NodeMcu 的 LUA API 将是一个好的开始。分线板只不过是用于 ESP8266、HC-05 和 Aux-1 连接的几个接头，带有几个电阻器、一个设置引导加载器模式的开关和一个 3.3V 调节器。如果您是 ESP8266 的新手，请使用由[Peter Jennings]撰写的这个[快速、方便的指南](http://benlo.com/esp8266/esp8266QuickStart.html)，开始使用 NodeMCU 和 Lualoader。[Chetan]在 ESP8266 上的 flash 代码，以及 Eagle board 设计文件可以通过他的 [Github repo](https://github.com/MakerChetan/3D-Printing-ESP8266) 获得。只需将代码闪存到 ESP8266 中，您就可以开始工作了。

需要注意的一个问题是在打印机启动后插入 ESP 模块。否则，来自 ESP 模块的初始通信会导致打印机锁定。我们确信这是可以通过改进分线板设计来解决的。也许可以使用斜坡板上 Arduino Mega 的数字信号，在启动期间暂时禁用 ESP 模块？休息后的视频给出了黑客攻击的简短概述。

[https://www.youtube.com/embed/aFH1TWNZgFk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/aFH1TWNZgFk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)