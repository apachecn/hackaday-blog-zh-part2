# 皮诺乔:把所有的东西(互联网)结合起来

> 原文：<https://hackaday.com/2014/07/15/pinoccio-mesh-all-the-internet-of-things/>

面向构建物联网的产品存在一个问题。每个构建硬件的人都需要投资者，因此需要某种方式来将他们的平台货币化。这意味着你所有的数据都被推送到“云端”，也就是你不拥有的服务器。这显然对黑客一族来说并不理想。是的，物联网可以通过几个廉价的无线电和一个被黑客入侵的路由器来完成，但你不会获得真实项目的所有酷功能-网状网络和设计良好的网络。 [Pinoccio](https://pinocc.io/) 是我们见到的第一个将适当的网状网络与您可以拥有的服务器结合在一起的产品。Pinoccio 团队非常友好，让我们上周末在 Rock City 时顺便访问，我们能够从[Sally]和[Eric]那里获得关于这些小电路板的独家新闻，以及他们可以做的非常酷的演示。

Pinoccio 上的硬件基本上是一个 Arduino Mega，带有一个 LiPo 电池和一个由 ATmega256RFR2 提供的 802.15.4 无线电。基板——技术上称为“野战侦察兵”——可以配备一个 WiFi 背包，作为 WiFi 网络的桥梁。这是一个非常聪明的解决方案，可以把大量的东西放到网络上，而不需要所有的东西都直接连接到互联网上。

当然，可以通过 Arduino 对这些球探进行编程，但 Pinoccio 的人还开发了一种叫做 ScoutScript 的东西，它允许你直接向网状网络上的任何或所有球探发送命令。有一个整洁的基于网络的图形用户界面，叫做 HQ，它允许你远程命令、控制和查询所有的小节点。

在下面的视频中，[Sally]介绍了硬件的基本功能及其功能。我们拜访时[Eric]在里诺，但他很友好地进行了视频聊天，并展示了 Pinoccios 网络的能力，每当他按下一个按钮时，就用 Hackaday 徽标装饰他们的网页。

[https://www.youtube.com/embed/GLER2I1r2-U?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/GLER2I1r2-U?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)