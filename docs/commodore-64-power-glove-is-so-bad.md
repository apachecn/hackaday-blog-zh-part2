# 准将 64 电力手套是如此糟糕

> 原文：<https://hackaday.com/2013/11/14/commodore-64-power-glove-is-so-bad/>

任天堂的力量手套太可怕了。真的真的很可怕。不过，多亏了现代组件，我们有可能以一种不那么糟糕的方式重现拳王手套的体验。这就是[叶小开]为准将 64 设计的动作感应手套所做的。

[叶小开]没有把自己的 IMU 卷起来放在手套里，而是使用 SonicWear SoMo，这是一种最初设计用来为演奏作品生成 MIDI 数据的手套。这只手套内有一个 9 自由度陀螺仪/加速度计/磁力计、uC、电池和 XBee，可以轻松重新编程，做一些比简单发送 MIDI 音符和命令更有用(或更不有用)的事情。

[叶小开]对 XBee 重新编程，使用 I/O 线传递，而不是发送串行数据，并通过一个非常简单的电路和一个十六进制反相器将接收 XBee 连接到 C64 操纵杆端口。

将 SonicWear 手套变成 C64 控制器的所有代码都可以在 Github 上找到[，还有](https://github.com/LeifBloomquist/SonicWear/tree/master/GamingGlove)[上个月底在 VCF 中西部展示他的手套的一个简洁的演示视频](http://www.ustream.tv/recorded/39334228)。