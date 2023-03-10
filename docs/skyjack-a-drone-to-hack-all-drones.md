# SkyJack:一架可以黑掉所有无人机的无人机

> 原文：<https://hackaday.com/2013/12/06/skyjack-a-drone-to-hack-all-drones/>

四轴飞行器逐渐变得更实惠，因而更受欢迎；我们预计今年假期会有比往年更多的孩子打开预制无人机。[Samy's]对充满无人机的未来有计划。他可能很快就会自豪地成为自己私人军队的新主人，因为他已经制造了一架无人机，可以同化他控制下的其他人。

这个建筑使用了一个鹦鹉 AR。无人机 2.0 带着一个附加的树莓 Pi 飞来飞去，它使用每个人都喜欢的[阿尔法适配器](http://www.alfa.com.tw/products_show.php?pc=34&ps=92)以混杂模式四处闲逛。如果 SkyJack 检测到一个分配给 Parrot 的 [IEEE 注册的 MAC](http://standards.ieee.org/develop/regauth/oui/oui.txt) 地址， [aircrack-ng](http://www.aircrack-ng.org/) 立即采取行动，向目标无人机发送认证请求，然后试图在原所有者重新连接时接管控制权。然而，任何成功套索的无人机都不会从天上掉下来。[Samy]使用 [node-ar-drone](http://github.com/felixge/node-ar-drone) 立即向从机发送新指令。

你可以在 GitHub 上找到他的所有代码[，但请确保你看到了下面的视频，它给出了全面的概述和简短的演示。还有一些其他的构建将](http://github.com/samyk/skyjack)[的树莓派捆绑到四轴飞行器](http://hackaday.com/2012/12/01/raspberry-pi-quadcopter/)上，值得一试；他们可以给你灵感，让你飞向天空。

[https://www.youtube.com/embed/EHKV01YQX_w?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/EHKV01YQX_w?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)