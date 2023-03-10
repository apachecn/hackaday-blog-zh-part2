# 用树莓皮听飞机应答器

> 原文：<https://hackaday.com/2013/05/23/listening-to-aircraft-transponders-with-a-raspberry-pi/>

去年的大黑客是软件定义无线电；一个小型 USB 电视调谐器，可以收听 64 到 1200 MHz 之间的任何地方的无线电广播。今年，一切都是关于树莓派，所以令人惊讶的是，我们只是现在才看到这两个硬件的混搭。正在使用 Raspi 和 RTLSDR 电视调谐器监听飞机转发器，并从头顶飞过的飞机上获得一大堆数据。

尽管 ADS-B 解码器[Corq]正在使用的[是为 OS X](http://www.blackcatsystems.com/software/cocoa1090.html) 编写的，但他正在通过网络用[一个名为 Dump1090](http://www.satsignal.eu/Radio/dump1090.html) 的程序读取来自 USB 电视调谐器的数据。这个程序允许[Corq]将他的 SDR 连接到一个 Raspbery Pi，并将其放在天线接收良好的地方——一个阁楼，或一个户外防风雨的箱子——并通过 WiFi 或网络连接将数据传输到他的桌面。

通过一个 USB 电视调谐器和一个 Raspberry Pi，[Corq]能够读取尾号、高度、纬度、经度、速度、航向，甚至是目前正在他家上空飞行的飞机类型。这很酷，但他可以通过互联网有效地做到这一点，这使得它成为一个出色的硬件混搭。