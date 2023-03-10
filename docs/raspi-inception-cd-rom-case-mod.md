# 拉斯皮“盗梦空间”光盘盒模型

> 原文：<https://hackaday.com/2014/02/01/raspi-inception-cd-rom-case-mod/>

![raspiInception](img/0df4df25daad798050bb465ff619ee3c.png)

乍一看，[John's] [CD-ROM RasPi case](http://blog.johndroach.com/2014/01/raspberry-pi-cd-rom-case.html) 似乎并不那么独特，但是我们喜欢它提供的实现和最终结果功能。他的目标是将 Pi 用作 torrent 下载器，并将下载的文件存储在共享的网络驱动器上。在服务器的情况下，Pi 驱动器将滑入一个隔间——因此有了 *Inception* 的参考:计算机中的计算机——允许下载，同时在服务器和外部世界之间放置另一个步骤，并保证网络共享可用，因为服务器和 Pi 将使用相同的电源。

[John]掏空了 CD-ROM 的内部，只留下了 PCB，除了后面的电源连接器，他几乎把所有东西都剥掉了。然后，他用他的旧 RasPi 盒的底部作为支架，将其安装到 CD-ROM 的 PCB 顶部。他将电源线焊接到 ROM 的电源连接器上，并临时连接了一个 5V 适配器，直到他让服务器运行起来。最后一步是切开外壳的背面，以便接入以太网和 USB 端口，这是[John]用 dremel、钢锯和锉刀完成的。外壳的正面看起来仍然像一个普通的 CD-ROM 驱动器，而[John]对未来的改进有计划:重新设计 LED 以显示网络活动，并修改按钮以作为 torrent 下载的重置、暂停或开始。