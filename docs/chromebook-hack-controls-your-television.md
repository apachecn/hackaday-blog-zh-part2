# Chromebook Hack 控制你的电视

> 原文：<https://hackaday.com/2013/04/29/chromebook-hack-controls-your-television/>

![chromebook_remote_control1](img/67cd03fba80b71448c47ba9129c706d9.png)

[迈克尔·科恩]只完成了他计划的一半，但我们仍然认为他的 Chromebook 电视频道切换器效果很好。在开始这个项目时，他希望包含一个列表网格，这样他就可以选择一个特定的程序，但是他认为搜集数据对于这个循环来说太麻烦了。

Chromebook 没有红外发射器，所以他用 MSP430 芯片制作了一个。他之前在 AVR 芯片周围建造了一个小发射器，并惊讶地发现其上的内部振荡器比 MSP430 上的精确得多。对于用于红外遥控器的曼彻斯特编码信号来说，时间就是一切，所以他用示波器尽可能精确地调谐 DCO。

屏幕上显示的应用程序是用 Javascript 编写的。Google 公布了一些在计算机上使用 RS232 的示例代码；[Michael]使用该资源来提供计算机和微控制器之间的通信。

[https://www.youtube.com/embed/oW_qJVzQhIg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/oW_qJVzQhIg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)