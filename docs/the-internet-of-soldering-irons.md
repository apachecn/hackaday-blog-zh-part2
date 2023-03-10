# 烙铁的互联网

> 原文：<https://hackaday.com/2015/07/19/the-internet-of-soldering-irons/>

物联网需要——嗯——东西。你真的需要把你的碎纸机连上互联网吗？也许吧。但是[Vegard Paulsen]在网络上放了一些每个黑客都能联系到的东西:[他的烙铁](https://vegardpaulsen.wordpress.com/2015/07/18/soldering-iron-and-nodemcu-iot-device)。

在典型的黑客风格中，修复焊接站上损坏的数字显示器变成了一个开发项目，允许[Vegard]在他的手机上监控他的烙铁的温度。他在空间站的 PC 板上找到了一个方便的电源，并连接了一个 NodeMCU WiFi 设备(使用无处不在的 ESP8266 和板载 Lua 解释器)。

数据被推送到 Thingspeak 服务器，该服务器负责将数据推送到更大的网络和数据表示(就像图中很酷的 Google gauge)。最棒的是:[Vegard]当他不小心忘了拿电烙铁时会收到电话通知。多完美啊。

他面临的一个独特挑战是将电源线焊接到焊台。这可能是一个问题，因为熨斗尖端是接地的，所以在熨斗通电时进行连接可能会烧断保险丝(或者更糟)。幸运的是，[维加德]未雨绸缪，设计了一个显然奏效的计划。

我们已经看到了其他例子，说明 NodeMCU 和 thing speak T1 如何轻松地将 T2 这个平凡的 T3 放到互联网上。不过，似乎用烙铁做工具特别合适。