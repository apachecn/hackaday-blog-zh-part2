# Xbox 控制器的电脑控制

> 原文：<https://hackaday.com/2012/04/20/computer-control-for-your-xbox-controller/>

![](img/706f8c7aebcaee04cd37610234ff8f9e.png "xbox-computer-controlled-controller")

这个布线噩梦让[H. Smeitink] [将 Xbox 360 控制器上的所有按钮映射到他的 PC 上](http://www.hmsprojects.com/xboxbypc.html)。这使他能够将控制输入从他的 PC 推送到控制台。但它比这更进一步，因为它实际上是一个直通设备。他将一个有线控制器连接到计算机上，并使用他编写的程序来翻译这些输入，并将它们发送到被黑客攻击的控制器。

软件是用 C#写的。它有一个录音功能，可以让他保存有线控制器上的按键数据，同时实时发送到 Xbox。当他找到一个他经常使用的组合时，他把那些命令提取出来，把它们设置成一个宏，然后分配一个按钮来执行它。控制器黑客为每个按钮使用一个晶体管，PIC 18F4550 控制它们并提供与 PC 的 USB 连接。

这不是一个像我们看到的[一些集成速射和宏解决方案](http://hackaday.com/2012/02/16/rapid-fire-update-brings-many-new-features/)那样的好包。但这无疑开启了更多的可能性。休息后在片段中自己看吧。

[https://www.youtube.com/embed/HKI311Ul92Y?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/HKI311Ul92Y?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)