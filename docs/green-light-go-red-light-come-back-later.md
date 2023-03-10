# 绿灯亮了就走，红灯晚了再回来

> 原文：<https://hackaday.com/2014/05/14/green-light-go-red-light-come-back-later/>

根据你对社交互动的品味和对分心的容忍度，一个开放式的平面图或“牛棚”办公室总共四个人可能并不坏。Hackaday.io 用户[fiddlythings]喜欢它，但人们经常停下来看他或他的一位同事，却发现他们很忙或不在。虽然他们的状态可以在自己的办公桌上从 Microsoft Communicator 中清楚地看到，但有些人喜欢亲自聊天，或者在参加会议和离开会议的路上停下来。

为了节省这些访客几秒钟的时间，[fiddlythings]利用他们现有的门外铭牌，设计了一个 [IM 状态指示器](http://hackaday.io/project/1014-IM-Status-Indicator-Nameplates)。他们每个人的名字旁边都有一个银色的小点，他用一个扁平的 RGB LED 背光照明。这些 led 由 Raspberry Pi 和 NPN 晶体管通过带状电缆驱动。

计划是模仿通信器的状态颜色，绿色表示可用，红色表示忙碌，黄色表示离开。[fiddlythings]用红色和绿色的混合调成了可爱的琥珀色。因为他实际上只需要两种颜色，所以他使用了八个 NPN 晶体管，而不是十二个。快速的概念验证版本使用了 Python 和一个名为[芬奇](https://developer.pidgin.im/wiki/Using%20Finch)的[洋泾浜 IM](http://pidgin.im/) 控制台客户端。一旦他得到许可，他就用 C++实现了最终版本，使用 [Libpurple](https://developer.pidgin.im/wiki/Using%20Libpurple) 与 Communicator 接口。

这不是我们第一次看到圆周率被用来表示状态——还记得这个移动黑客空间指示器吗？