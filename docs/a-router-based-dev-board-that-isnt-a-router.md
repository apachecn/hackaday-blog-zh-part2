# 不是路由器的基于路由器的开发板

> 原文：<https://hackaday.com/2014/07/27/a-router-based-dev-board-that-isnt-a-router/>

这里有一些东西会让那些希望为自己的联网项目或物联网实施而破解路由器的人感兴趣:基于相当标准的路由器的硬件，加载了 OpenWRT，有大量的 I/O 来连接任何东西。

它被称为 DPT 板，它基本上是你可以通过通常的渠道买到的现成路由器的巨大改进版本。板载 20 个 GPIOs、USB 主机、16MB 闪存、64MB RAM、两个以太网端口、板载 802.11n 和一个 USB 主机端口。这个板上的小系统预装了 OpenWRT，可以相对容易地将这个类似路由器的小设备连接到 led 灯条、传感器或您想到的任何其他项目。

该板由[金奎大·佩普]设计，他还在研究一种他称之为[突破服务器](https://github.com/dptechnics/breakoutserver)的东西。有一种专门为该板编写的 uHTTP 服务器，允许任何联网设备控制板上的一切。他们还在开发一款 HTML5 应用，可能会非常有趣。

总而言之，这是一个非常酷的小设备，很好地介于相对简单的“带以太网屏蔽的 Arduino”和 Raspi 或 BeagleBone 之间。