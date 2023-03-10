# 将 AirPlay 添加到货架系统

> 原文：<https://hackaday.com/2013/01/08/adding-airplay-to-a-shelf-system/>

![adding-airplay-to-a-shelf-system](img/54291ce98a169c3be17e2103904f5ba6.png)

AirPlay 是一个很棒的系统。它允许你将正在播放的任何媒体从一个设备发送到另一个设备。当然，我们希望它能更开放一点(苹果当然不知道这一点)，但有几个选择来创建自己 AirPlay 接收器。在遇到一个能做到这一点的项目后，[马特·雪莉]决定把他的架子系统变成一个 AirPlay 接收器。

实现他的目标的途径取决于 Raspberry Pi 使用 Shairport 包接收 AirPlay 音频的能力(我们上周刚刚看了另一个做这个的玩家)。他使用 Edirol UA-5 USB 音频接口作为他的唱机的放大器。他没有使用 USB 端口，并且知道连接 RPi USB 作为设备的主机很简单。

为了保持系统的外观尽可能干净，他打开了扩音器的盖子。有足够的空间将小 RPi 板放在里面。他在金属外壳的侧面开了一个 USB 端口的开口(真的，看图片)。一根短插线从一个端口连接到放大器背面的 USB 插孔。离开箱子侧面的白色电缆为 Rasperry Pi 供电。手术很成功，现在他可以用手指轻轻一敲就能听到自己的曲子了。