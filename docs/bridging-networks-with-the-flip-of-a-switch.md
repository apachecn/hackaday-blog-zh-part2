# 通过开关的翻转来桥接网络

> 原文：<https://hackaday.com/2014/11/16/bridging-networks-with-the-flip-of-a-switch/>

TP-Link TL-WR703n 是现代的 wrt 54g——非常容易破解，非常便宜，几乎随处可得。装载了 OpenWRT，它能够桥接网络:将以太网转换成 WiFi，反之亦然。这需要重新配置路由器，在这样做了足够多次之后，[【Martin】正在寻找更好的解决方案](http://www.martinmelchior.be/2014/11/configure-your-wr703n-with-switch-or-two.html)。WR703n 内部的 SOC 有两个外露的 GPIO 引脚，允许[Martin]在 WiFi 接入点或客户端以及桥接或 NAT/DHCP 之间进行选择。

根据 OpenWRT wiki 的[，有一些 GPIOs 可用，在将这些引脚连接到 DIP 开关后，【Martin】可以通过固件访问这些开关。这个构建的难点是构建脚本，以便在系统启动时更改设置。这个脚本查看 GPIOs 的状态，将 WiFi 更改为客户端或接入点模式，并尝试不在云中的某个地方使用 DHCP。是的，我们只是在适当的上下文中使用了云。](http://wiki.openwrt.org/toh/tp-link/tl-wr703n)

完成这一构建的唯一其他硬件是一个简单的 USB 到串行转换器，它应该被推到每个人工作台的角落里。对于一个极其有用的东西所需要的极小的焊接和配置来说，这已经不错了。