# 用于图形计算器的 GPS

> 原文：<https://hackaday.com/2014/02/04/gps-for-a-graphing-calculator/>

![GPS](img/2e9c6bc2bc542731eda6a8ba0490ad7a.png)[Chris]是一名杰出的图形计算器黑客，他的几个项目出现在了 Hackaday 的首页，主要是将如上图所示的 TI-84 Plus 这样的图形计算器转化为复制智能手机的一些功能。他的最新建造，[一个附加在 TI-84 加](http://www.cemetech.net/projects/item.php?id=51) 上的硬件 GPS 模块，是他在经典硬件之外的又一个令人敬畏而不切实际的帽子上的羽毛。

将 GPS 添加到图形计算器中有两个主要的技术挑战。第一个是给 GPS 传感器供电。许多计算器改装者已经做了大量工作来记录 84 Plus 上的 USB 端口，揭示它是一个 USB OTG 端口，能够作为主机或设备。它还为几乎任何东西提供 5V 的电源，结果烧坏了电池。

下一个挑战是以 4800bps 的速度读取来自 GPS 传感器的数据。TI-84 Plus 系列计算器有一系列中断，可以在 15MHz 时钟的几分之一处触发。通过将计时器设置为每 197 个时钟周期触发一次，并再次除以 16，[Chris]可以以 4758.9bps 的速度读取数据。这足以获取大部分数据，NMEA 协议中包含的校验和允许软件丢弃错误的消息。

[https://www.youtube.com/embed/u_kLtYNJOqA?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/u_kLtYNJOqA?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)