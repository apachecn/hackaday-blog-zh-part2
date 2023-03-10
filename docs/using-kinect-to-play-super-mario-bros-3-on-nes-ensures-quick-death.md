# 在 NES 上用 Kinect 玩超级马里奥兄弟 3 确保快速死亡

> 原文：<https://hackaday.com/2014/10/25/using-kinect-to-play-super-mario-bros-3-on-nes-ensures-quick-death/>

为什么只有新的游戏主机才能获得所有很酷的外设？作为一个实干家，[保罗]着手改变这种状况。他有一台 Kinect V2 和一台原版任天堂游戏机，他认为让这两者一起工作会很有趣。

考虑到模仿一个标准的控制器是最容易的，[Paul]在网上浏览了一下，直到他发现了一篇精彩的文章，解释了 NES 控制器是如何工作的。原来，除了按钮之外，控制器中只有一个移位寄存器芯片和一些上拉电阻。他决定将另一个移位寄存器和一些电阻粘在一块试验板上，用控制器电缆直接连接芯片，而不是焊接成一个拆下来的 NES 控制器。

![Kinect4NES wiring](img/cf84ab35709c56929e02b79de54f19bc.png)

Arduino 用于模拟按钮的按压。Arduino 正在运行 Firmata sketch，它允许从主机切换 Arduino 引脚。那台主机运行着[保罗]用 Kinect V2 SDK 自己编写的应用程序，该程序将玩家的手势转换成控制器命令，然后告诉 Arduino“按”哪个按钮。这绝对是一个非常有趣和复杂的项目，即使这个视频让从布瑟和库佩林斯手中救出毒菌公主看起来非常具有挑战性！

如果你想帮助这个项目或者只是为你自己建一个，请在 GitHub 页面查看源文件。

[https://www.youtube.com/embed/5LQ7ks8HfQA?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&start=59&wmode=transparent](https://www.youtube.com/embed/5LQ7ks8HfQA?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&start=59&wmode=transparent)