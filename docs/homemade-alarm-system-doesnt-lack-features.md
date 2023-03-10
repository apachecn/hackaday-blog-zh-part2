# 自制警报系统不缺乏功能

> 原文：<https://hackaday.com/2014/05/30/homemade-alarm-system-doesnt-lack-features/>

![alarm system](img/63df520ebef14b36275b1ae95c2272dd.png)

对我们许多人来说，我们的车库(或工作室)可能是房子最重要的部分之一。如果窃贼破门而入，我们可能会更担心我们的工具！[Ron Czapala]决定在他的车库里需要一个警报系统来保证他的东西的安全，所以他决定从头开始建造一个。

该系统利用视差 4×4 键盘膜、MCP23008 端口扩展器、视差推进器、LCD 屏幕和一些开关来代表位于门和窗户中的未来磁簧开关。

使用循环缓冲器，推进器有几个状态来监控车库。

*   未装备—忽略所有传感器
*   待命—系统将对传感器的变化做出反应
*   退出延迟—系统已启动，45 秒倒计时开始，允许您退出车库
*   窗户触发器—如果窗户被打开，警报将立即响起(警报器和闪光灯)
*   门触发器—如果没有在键盘上输入正确的代码，警报将在 60 秒后响起

要获得完整的演示，请查看下面的视频，其中[Ron]解释了这一切！

[https://www.youtube.com/embed/plLQFZlsKHA?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/plLQFZlsKHA?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

你知道什么更适合你家的警报系统吗？激光。看看这个[激光绊线报警器！](http://hackaday.com/2011/03/11/passcode-protected-laser-tripwire-alarm-system/)

【谢谢安德鲁！]