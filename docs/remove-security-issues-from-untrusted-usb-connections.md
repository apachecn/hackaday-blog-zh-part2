# 消除不受信任的 USB 连接的安全问题

> 原文：<https://hackaday.com/2015/06/23/remove-security-issues-from-untrusted-usb-connections/>

如今，USB 已经变得相当“通用”，可以处理从高速数据传输到手机充电的一切事情。甚至还有 USB 供电的熔岩灯。然而，这种无处不在的现象并不是没有代价的。智能手机和电脑上有许多攻击，它们利用了 USB 几乎无处不在的事实，如果你想避免这些攻击，你可以放弃使用 USB，或者像[Jason]那样[阻塞 USB 端口](http://www.reclaimerlabs.com/blog/2015/6/2/charging-safely-over-usb)上的数据线。

USB 通常使用四根线:两根用于电源，两根用于数据。但是，如果你只是简单地断开数据线，外围设备就无法与主机协商更多的功率，只能勉强维持 0.5 瓦的功率。然而，[Jason]发现这种协商的数据传输速率比正常数据传输速率低得多，并且能够在主机和外设之间放置一种过滤器。滤波器允许低频数据传输通过，但当高频数据传输发生时，滤波器会阻止通信。

[Jason]现在有一款设备可以让他的外围设备以更高的速率充电，而不必担心不可信的 USB 端口(例如，在机场或咖啡店)。这个简单的装置可以阻止像 BadUSB 这样的东西做肮脏的工作，尽管它是否能阻止 T2 这样令人讨厌的东西仍然悬而未决。