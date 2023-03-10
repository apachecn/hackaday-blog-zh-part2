# 经典的 80 年代立体声接收机享有第二次生命作为收音机

> 原文：<https://hackaday.com/2013/11/06/classic-80s-stereo-receiver-enjoys-a-second-life-as-radioduinowrt/>

![radio2](img/cc310052f628a38656d54105d04e2d4c.png)[raff ael]有一个破旧的雅马哈自然声音接收器。T2 没有扔掉它，而是为自己建造了一个漂亮的网络收音机 T4。他称之为无线电广播。[Raffael]从移除所有内部构件开始——尽管他保留了前面板控制。然后他添加了一个 Arduino Mega 来处理前面板控制，包括一个 16×2 字符的 LCD 模块。Arduino 还通过红外遥控器接收命令。enc28j60 以太网模块允许 Arduino 与操作的大脑 TL-WR703N 迷你路由器进行通信。

一个微型 USB 集线器扩展了 WR703 上的单个 USB 端口，允许安装 USB 声卡和 4g USB 记忆棒。我们想补充的是，TL-WR703 在这个应用中是一个必须的链接——亚马逊链接(Rafael)提供了一个顶部链接——T2 TL-wr 702(T3)。只有 TL-WR703 有 USB 主机连接。

真正的魔力在于[拉斐尔的]软件设置。WR703 运行的是 OpenWRT。他为 USB 声卡添加了模块，并将文件系统扩展到 u 盘上。一旦完成,[Raffael]添加了[音乐播放器守护程序(MPD)](http://www.musicpd.org/) 和 MPC，一个驱动 MPD 的控制台应用程序。Lighttpd 是一个轻量级 web 服务器，它为 Arduino 提供了一个接口，同时也是整个无线电的 web 前端。所有这些都允许[拉斐尔]以多种方式控制他的收音机。他可以通过网络上的任何浏览器登录。他可以使用前面板控制。他可以使用红外遥控器。由于他是 MPD 的负责人，[任何客户](http://mpd.wikia.com/wiki/Clients)(实际上有数百个)也将驱动无线电。

虽然家庭立体声应用中的低端 USB 声卡确实让我们内心的高保真音响发烧友有点畏缩，但质量似乎确实不错。Rafael 的设计使得在需要的时候更换更高质量的 USB 声卡变得简单。

[https://www.youtube.com/embed/XZhS7eKzMSA?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/XZhS7eKzMSA?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)