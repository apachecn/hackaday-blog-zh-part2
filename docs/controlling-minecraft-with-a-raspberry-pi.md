# 用现实生活中的红石控制树莓派

> 原文：<https://hackaday.com/2013/01/30/controlling-minecraft-with-a-raspberry-pi/>

![minepi](img/21d483a2422ac386b558764ad083d562.png)

我们已经看到在《我的世界》用红石建造的计算机，红石是游戏中的电、电路和数字逻辑。我们甚至已经看到一些红石的装置控制现实世界的设备。[安格斯]“建造，虽然，把事情带到了一个全新的水平。他用树莓派在《我的世界》赛道和现实生活中的赛道之间架起了一座桥梁。

[Angus]“构建依赖于作为 Bukkit 插件运行的《我的世界》服务器的 mod。由 redstone 驱动的块标有游戏内标志，关于块状态的消息使用 [MQTT 协议](http://mqtt.org/)通过网络传递。

构建的硬件方面是带有 PiFace 扩展板的 Raspberry Pi。通过这种设置，[Angus]可以通过切换《我的世界》杆来控制 PiFace 上的 led，或者使用 PiFace 的按钮点亮红石灯。

如果你想亲自尝试一下，你可以在[【安格斯】的 git](https://github.com/ajtag/ReallifeRedstone) 上下载 Bukkit 插件。休息之后，请查看现实生活中雷石东的视频。

[https://www.youtube.com/embed/ythrmFAJugw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/ythrmFAJugw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)