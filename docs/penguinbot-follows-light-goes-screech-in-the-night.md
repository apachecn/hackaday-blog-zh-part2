# 企鹅号跟着光，在夜晚发出刺耳的声音

> 原文：<https://hackaday.com/2014/04/18/penguinbot-follows-light-goes-screech-in-the-night/>

曾经有过这样一个周末项目，它有自己的生命吗？做了，结果是这个[企鹅机器人](http://arduino-pi.blogspot.ca/2014/04/penguinbot-fun-weekend-arduino-project.html)。当[迈克尔的]妻子外出度周末时，他偶然发现了一只坏了的玩具企鹅。电池漏了进去，损坏了触点。迈克尔没有把这个玩具扔掉，而是把它变成了一个自主机器人。[迈克尔]的目标是创造一个机器人，它可以在房子里漫游，避开障碍物，或者跟随像手电筒一样的光源。

他从取出大部分原始电子设备开始。两个一元店的玩具火车献出了自己的生命和自己的马达来代替企鹅原来的驱动系统。一台 Arduino Pro Mini 成为了 PenguinBot 的大脑。传感器由两个光敏 CdS 电池、一个 AdaFruit 声音传感器和一个 MaxBotix 超声波传感器组成。由于超声波传感器安装在伺服系统上，它可以检测任何方向的障碍物。CdS 电池和一些软件将允许企鹅机器人像任何优秀的摄影机器人一样跟随光线。

点击休息时间，观看企鹅机器人的运行

![The PenguinBot's internals laid out for all to see](img/53d1ff97dbbbc464a825ae0ee9398474.png)

[迈克尔]确实保留了原玩具的一部分。企鹅机器人仍然有它的声音模块。这东西太吵了，太棒了。在尖叫声和随机歌曲之间，[迈克尔的]孩子们不用担心他们的新机器企鹅会在晚上偷偷靠近他们。

PenguinBot 的代码仍在开发中，但最新版本可以在 [Github](https://github.com/michaeljball/PenguinBot) 下载。

[https://www.youtube.com/embed/p4hGA2_M8Ak?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/p4hGA2_M8Ak?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/cYCboZXBxdE?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/cYCboZXBxdE?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/ECWfho7n_M0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/ECWfho7n_M0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)