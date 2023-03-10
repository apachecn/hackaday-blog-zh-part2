# ProxyGambit 优于 ProxyHam 带咖啡店 WiFi 全球

> 原文：<https://hackaday.com/2015/07/16/proxygambit-better-than-proxyham-takes-coffee-shop-wifi-global/>

上周末发布了 ProxyHam，这是一种通过 900MHz 无线电链路从公共图书馆和咖啡馆跳到 WiFi 上来匿名化互联网活动的设备。该项目神秘地消失了，并从防御计划中删除。没有人知道为什么，但是我们花了一些时间推测这个秘密版本中实际使用了什么硬件。

[Samy Kamkar]刚刚通过 ProxyGambit 改进了 ProxyHam 概念，[这是一种将您的位置与您的 IP 地址](http://samy.pl/proxygambit/)分离的设备。但是[萨米]的建造并不局限于 ProxyHam 声称的两英里范围。ProxyGambit 可以通过 2G 连接在地球上的任何地方工作，或者通过视距点对点无线链接在 10 公里(6 英里)以外工作。

ProxyGambit 的 more GSM 版本使用两个 Adafruit FONA GSM 分线板、两个 Arduinos 和两个 Raspberry Pis。FONA 板通过 2G 产生出站 TCP 连接。Arduino 用作反向 TCP 隧道上的串行连接，并直接连接到 Raspberry Pi 的 UART。Pi 只是连接两端的一个网桥。通过在构建的“一次性”部分建立 TCP 连接的反向隧道，[Samy]可以在任何有 2G 服务的地方获得互联网连接。

虽然这只是一个概念证明，不应该被任何真正需要匿名的人使用，但是 ProxyGambit 确实比 ProxyHam 有一些优势。它几乎可以在地球上的任何地方使用，而不仅仅是在公共 WiFi 接入点的两英里范围内。【ProxyGambit 的来源也是可用的，一些永远不会说的 ProxyHam 的东西。