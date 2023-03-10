# 为 Klipsch 环绕声系统添加遥控器

> 原文：<https://hackaday.com/2012/06/07/adding-remote-control-to-klipsch-surround-system/>

![](img/2791d69d63ff1fef51745fc76e11614c.png "adding-remote-control-to-surround-system")

[Zurcher]购买的扬声器系统是 Klipsch 制造的。这是一个环绕声单元，但它旨在与计算机一起使用，因此没有无线遥控器。取而代之的是，一个有线单元放在桌子上，让你在扬声器或耳机之间进行选择，并有一个音量调节旋钮。问题是他将它们用于他的家庭影院系统，并且[不得不添加他自己的遥控硬件](http://christopherzurcher.blogspot.com/2012/05/klipsch-promedia-51-volume-control-pod.html)来从房间的另一端调整它们。

他从一些非常有用的网络搜索开始。似乎其他人已经在过去绘制了硬件，他能够使用这些信息找到控制器内部的音量芯片。稍微嗅一下信号，他就能计算出 i2c 总线上的控制命令。这是他建造自己的控制器所需的信息。他拿起他的 Arduino 板和红外接收器，几乎可以从任何遥控器接收命令，还有一个四位数的 7 段显示器，可以提供设置反馈。休息之后，你可以看到他在视频中展示了最终的造型。

[https://www.youtube.com/embed/12ISjwoT09M?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/12ISjwoT09M?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)