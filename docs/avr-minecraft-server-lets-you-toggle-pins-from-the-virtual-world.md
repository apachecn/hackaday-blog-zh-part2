# AVR《我的世界》服务器让你从虚拟世界切换引脚

> 原文：<https://hackaday.com/2012/11/16/avr-minecraft-server-lets-you-toggle-pins-from-the-virtual-world/>

想要通过建立一个网络服务器来测试他的技能[Cnlohr]决定也编码[一个《我的世界》服务器，允许他从游戏内部切换 pin 码](https://github.com/cnlohr/avrcraft)。上面看到的成排开关使他能够直接访问 ATmega328 一个端口的方向寄存器和 I/O 引脚。

服务器硬件如上图所示。仅仅从图像上很难判断，但它实际上是一种玻璃基板，是 Cnlohr 的专业产品。他使用 ENC424J600 来处理网络方面的事情。这种芯片的价格几乎是旁边微控制器的两倍。但即使是单个数量，整个版本的 BOM 也不到 20 美元。

在休息之后的视频中，Cnlohr 和一个朋友展示了多用户登录《我的世界》世界的能力。该模拟相当简单，但从游戏世界影响硬件的能力比仅仅通过一些双绞线推动 1 和 0 更令人兴奋。

[https://www.youtube.com/embed/EZRLOanNQ_w?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/EZRLOanNQ_w?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[via [Reddit](http://www.reddit.com/r/electronics/comments/138cvg/minecraft_server_on_a_microscope_slide_youtube/)