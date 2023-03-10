# 获得一个控制台和运行在树莓皮上的雷神之锤 2

> 原文：<https://hackaday.com/2012/07/02/getting-a-console-and-quake-ii-running-on-a-raspberry-pi/>

![](img/794e2a7cc7176c618443644fe411af74.png "raspi")

那些 Raspberry Pi 板正在飞向全球各地修补匠的邮箱，所以我们的提示线目前被淹没在 Raspi hacks 的洪流中。这是周末收到的两条消息:

首先是[reefab]的雷神之锤第二版的树莓码头。建造是基于[山木地震 2](http://www.yamagi.org/quake2/)和*大部分*可玩。雷神之锤 III 的树莓派[端口已经过时了](http://www.raspberrypi.org/archives/1139)，但是我们很乐意随时重温雷神之锤 II 的刺激动作。

接下来是[Joonas]'接手[获得一个串行控制台并用 Raspi 运行](http://codeandlife.com/2012/07/01/raspberry-pi-serial-console-with-max3232cpe/)。Raspberry Pi 的 26 针接头上有一个 UART 串行控制台，但您不能只将这些针连接到串行端口。为了将+/- 12V 下调到 Raspi 可以理解的 3.3 伏，[Joonas]使用了 max 3232——每个人都喜欢的 RS-232 收发器的 3.3 伏版本。有了试验板和几个盖子，就可以很容易地将您的 Raspi 连接到串行控制台。干净利落。