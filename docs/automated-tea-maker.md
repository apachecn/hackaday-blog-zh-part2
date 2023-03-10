# 自动泡茶机

> 原文：<https://hackaday.com/2015/01/28/automated-tea-maker/>

[Pariprohus]想给他的女朋友做一个有趣的礼物。他知道自己泡茶有多困难，于是决定制造一个小机器人来帮忙。他的自动化泡茶器很简单，但是很有效。

该设备由 Arduino Nano 驱动。Nano 连接到一个伺服系统、一个压电扬声器、一个 LED 和一个开关。当开关转到关闭位置时，伺服旋转到“折叠”位置。这将浸泡臂移动到一个位置，使设备更容易储存和运输。

当设备打开到“就绪”位置时，机械臂将向外伸出并保持不动。这给了你时间将茶包系在手臂上，并将一杯热水放在下面。最后，可以将交换机置于“brew”模式。在这种模式下，袋子被放入热水中并保持大约五分钟。每一分钟袋子都被举起和放下来搅动周围的水。

一旦循环完成，Nano 就会从[压电扬声器](http://hackaday.com/2012/09/15/how-to-make-your-own-piezoelectric-speaker/ "DIY piezo speaker")播放音乐，提醒你喝新沏的茶。包括音乐在内的所有参数都可以在 Nano 的源代码中修改。所有的部件都装在一个漆成白色的小木箱里。看看下面的视频，看看它的作用。

[https://www.youtube.com/embed/MWL4pxy24Ak?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/MWL4pxy24Ak?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)