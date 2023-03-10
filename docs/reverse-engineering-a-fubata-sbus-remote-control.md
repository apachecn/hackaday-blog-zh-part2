# 逆向工程双叶 SBUS 遥控器

> 原文：<https://hackaday.com/2012/04/05/reverse-engineering-a-fubata-sbus-remote-control/>

![](img/1c9082df62ce1fc04d31457d1f63a141.png "Fubata")

在航模界，双叶的 SBUS 系统是一件大事。SBUS 系统允许每个接收器有 16 个比例控制和两个数字通道，而不是每个通道有一个伺服系统。基本上，如果你正在建造一架起落架和炸弹舱门都缩回的超棒的飞机，这就是你想要使用的。[迈克尔]想在他正在进行的项目中使用一些 SBUS 伺服系统，所以他当然必须对这个专有协议进行逆向工程。

每个 SBUS 伺服都通过一个 100kbps 的串行连接运行，其中有一些有趣的变化:信号以大端字节序传输，但单个字节是小端字节序，这是[Michael]在偶然发现本月旧的 mbed 帖子后发现的。[Michael]使用了由[fat16lib]编写的串行库，并且能够通过一个简单的十六进制反相器改变奇偶校验位和停止位。当伺服连接到一个 Arduino Mini 时，一切都完美地工作。

尽管 SBUS 系统需要[特殊的双叶伺服系统](http://www.futaba-rc.com/servos/sbus.html)，我们可以很容易地看到【迈克尔】的工作对于异常复杂的机器人或数控机器是多么有用。休息之后，请观看视频，快速演示[Michael]的试验板控制其中一个 SBUS 伺服系统。

[https://www.youtube.com/embed/_qeLBebtsdw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/_qeLBebtsdw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)