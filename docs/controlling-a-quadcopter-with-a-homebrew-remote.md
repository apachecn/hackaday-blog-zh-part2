# 用自制遥控器控制四轴飞行器

> 原文：<https://hackaday.com/2012/08/22/controlling-a-quadcopter-with-a-homebrew-remote/>

![](img/31e76de42eb8f696122597649c041f85.png "RC")

当[马特]开始建造他的多旋翼直升机时，他太专注于建造他的飞行器，而不是担心如何实际控制他的直升机这样的小细节。不过，最后一切都解决了，这要感谢[他用 USB 操纵杆和几个 XBees 构建的自制 RC 设置](http://aimatt.com/2012/08/02/diy-rc-receiver-serial-ppm/)。

经过一些最初的修改和在多转子 IRC 房间的大量聊天后，[Matt]无意中发现了将[脉冲位置调制](http://en.wikipedia.org/wiki/Pulse-position_modulation)用于他的无线电控制设置的想法。

经过几次修改后，[Matt]决定使用 Arduino Pro Mini 作为他的飞行电脑，搭配一个无线模块。通过将他的多架直升机置于特设模式，他可以通过 WiFi 用笔记本电脑连接到直升机，并发送命令，而不需要第二个 XBee。

现在，每当[马特]想要驾驶他的多翼飞机时，他就将 WiFly 模块插入他的 [MultiWii 板](http://www.multiwii.com/)，将他的笔记本电脑连接到直升机，并运行一个小的 Python 脚本。这可能不会比买一个漂亮的双叶发射机更容易，但随着他的直升机队能力的增长，[马特]可以很容易地扩展他的设置。

休息后，[马特]的直升机在飞行中的视频。

[https://www.youtube.com/embed/_Q5dbNigOiQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/_Q5dbNigOiQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)