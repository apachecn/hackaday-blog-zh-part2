# 为你的家用电器提供口哨控制

> 原文：<https://hackaday.com/2012/04/02/whistle-controls-for-you-home-electronics/>

![](img/58d42527f5427e247115f34f94c63016.png "whistle-controlled-devices")

你知道怎么吹口哨，不是吗？你只要把嘴唇合拢，然后吹气。但是你知道如何让你周围的电子设备对你吹口哨的命令做出反应吗？嗯,[Befi]想出了一个系统，可以让他给各种家用电器分配一个口哨命令。

他正在使用一套射频遥控插座来切换各种设备的电源，如办公桌或转台。你在上面的图像中看到的电路板是系统自带的遥控器，但那个芯片是他添加的 ATmega8，使用串行到 USB 转换器提供 USB 连接。这项技术非常简单，我们打赌你可以让它与 ATtiny2313 和 V-USB 项目一起工作，但这是另一个故事了。

额外的部分是使用嵌入式 Linux 来检测和处理吹口哨的命令。在休息后的视频中，[Befi]解释说他正在使用 Dockstar 和麦克风来捕捉音频输入。它使用快速傅立叶变换算法来处理剪辑，并在处理完成后将命令推送到遥控器。[https://www.youtube.com/embed/KpZeG4NNxx0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/KpZeG4NNxx0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)