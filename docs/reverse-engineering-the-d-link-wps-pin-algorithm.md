# 对 D-Link WPS Pin 算法进行逆向工程

> 原文：<https://hackaday.com/2014/10/31/reverse-engineering-the-d-link-wps-pin-algorithm/>

![sub_4D56F8](img/33c754dab893e1a1202a0f9b618548fb.png)

带有 WPS 的路由器需要一个 PIN 码来允许其他设备连接，并且该 PIN 码对于每台路由器都应该是唯一的，而不是从路由器上其他容易访问的数据中派生出来的。当[Craig]查看一个 D-Link DIR-810L 802.11ac 路由器的固件时，[他发现了完全相反的](http://www.devttys0.com/2014/10/reversing-d-links-wps-pin-algorithm/)；WPS PIN 码*很容易被*破译，因为它完全是从路由器的 MAC 地址生成的，可以通过嗅探 WiFi 进行逆向工程。

当[Craig]查看从他的路由器上拆卸下来的固件时，他注意到一段代码访问了用于存储设备特定信息(如序列号)的 NVRAM。这段代码*不是*获取 WPS pin，而是 WAN MAC 地址。WPS pin 不是对每台设备都是唯一的，对路由器上的每一位数据都是不透明的，而是简单地从 MAC 地址生成(用一点数学运算)。这意味着路由器上游的任何人都可以很容易地获得路由器的 WPS pin，并且实质上给了每个人打开这个路由器城堡的钥匙。

几年前，人们发现 WPS pin 无论如何都是极不安全的，[能够在几分钟内被暴力破解](https://code.google.com/p/reaver-wps/)。路由器制造商可以应用一些补丁来检测这些暴力攻击，从而消除这个漏洞。[Craig]的代码表明，大量的 D-Link 路由器有效地向全世界广播了它们的 WPS PIN。更糟糕的是，每个无线帧中的 BSSID 也是从 WAN MAC 地址中获得的。[Craig]已经破解了大量 D-Link 路由器上的 WPS，这要感谢一位工程师决定从 MAC 地址生成 WPS PIN。

[Craig] [有一个不完整的列表，列出了他的站点上确认受影响的路由器](http://www.devttys0.com/2014/10/reversing-d-links-wps-pin-algorithm/)，以及一个确认未受影响的路由器列表。