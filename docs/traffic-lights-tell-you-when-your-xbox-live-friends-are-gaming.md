# 当您的 Xbox Live 朋友在玩游戏时，红绿灯会告诉您

> 原文：<https://hackaday.com/2012/10/01/traffic-lights-tell-you-when-your-xbox-live-friends-are-gaming/>

![](img/725ce2e5a490c9258eb6ccddb32dc67a.png "xbox-live-traffic-lights")

这听起来像是(安德鲁)试图在他的行为中建立一个巴甫洛夫反应，当涉及到网络游戏的时候。他想确保当他所有的朋友都在线时，他不会错过，所以[他建立了这个交通信号来监控 Xbox Live](http://handya.co.nz/post/32580478459/xbox-live-traffic-lights) 的活动。它会点亮灯，并根据他的哪些朋友当前在线来驱动不同的仪表。绿灯亮的时候，他放下一切，抓起一个控制器。

灯光的底座是一个黑色的投影盒。在里面你会发现一个 Arduino 兼容芯片，它驱动安装在一块原型板上的设备。WIZnet W5100 以大约 25 美元的低价增加了网络连接。设置有一个问题。[Andrew]找到的 API 不使用任何身份验证。这意味着他只能看到好友的公开状态；任何将其在线状态设置为“私人”的人将始终注册为“在线”。如果你知道现有的 Xbox Live API 可以解决这个问题，我们希望在评论中听到你的意见。