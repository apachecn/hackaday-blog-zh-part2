# RFID 仿真卡包括一个学习模式

> 原文：<https://hackaday.com/2013/01/18/rfid-emulator-card-includes-a-learning-mode/>

![rfid-emulator](img/e3d10a0e8fc19a42e35606ceea4bcd98.png)

这张射频识别卡有很多很好的功能。但是最突出的是从另一个 RFID 标签或卡片学习代码的能力。

你可以看到电路板上有一个蚀刻线圈，用来与 RFID 阅读器互动。这是该器件的唯一电源，使其能够从阅读器获得足够的感应电流，为电路板左上角的 PIC 12F683 供电。PCB 的底部只有三个组件:一个 LED 和两个开关。其中一个开关将设备置于学习模式。当你把板子移到阅读器的磁场中时，只要按住那个按钮就行了。而在学习模式中，第二个 RFID 标签被举向读取器。它将识别自己，仿真器将捕获在交互过程中发送的代码。休息后的视频中显示了这一切。我们想知道，当仿真器举到读者面前时，通过按住不同的按钮来存储几个不同的代码会有多难？

如果你也想建造自己的读卡器，这里有一个项目可以从头开始。

[https://www.youtube.com/embed/TRRJnnJuObg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/TRRJnnJuObg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)