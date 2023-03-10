# GLCD 时钟项目包含了很棒的用户界面和特性

> 原文：<https://hackaday.com/2013/02/11/glcd-clock-project-packed-with-great-ui-and-features/>

![glcd-clock-packed-with-features](img/39f53795edfb66c8003a759525545848.png)

这款[图形液晶时钟](http://www.redstardesignbureau.com/web_clock/Clock.html)没有花哨的外壳，但【Gregory Wright】内置了如此多的出色功能，我们认为它将成为未来许多项目的灵感来源。如果他决定添加一个案例，这将是非常容易的，因为没有按钮来工作。

没有按钮，东西怎么调节？他决定用红外遥控器来控制所有的设置。这给了他比几个按钮更多的选择。另外，深度睡眠者需要找到遥控器来关闭闹钟。我们还认为有趣的是，他使用的 595 移位寄存器具有足够低的数据高阈值(当 VCC 为 4.5V 时为 3.15V)，因此他不需要电平转换器来驱动 3.3V MSP430 Launchpad 的 5V 显示器。

休息之后看看他的视频，了解他在 UI 中包含的所有功能。我们最喜欢的显示在右下角，那里写着“你好，世界”。这是一个专用于每天定制消息的区域。他用它来提醒自己垃圾日(现在有一个功能！).

[https://www.youtube.com/embed/UOkbphLlNbE?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/UOkbphLlNbE?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)