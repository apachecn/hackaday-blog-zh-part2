# HOPE X:无线 Tor 代理和共享 TrueCrypt 卷

> 原文：<https://hackaday.com/2014/07/23/brazilonion/>

[https://www.youtube.com/embed/DE72vayz2TY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/DE72vayz2TY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

当你在 HOPE 的时候，你当然会看到一些 Tor 代理，但是(Jose)的是顶级的。这是一个完全可移植的 Tor 代理。br，[谷歌翻译](https://translate.google.com/translate?sl=pt&tl=en&js=y&prev=_t&hl=en&ie=UTF-8&u=http%3A%2F%2Fwww.area31.net.br%2Fwiki%2FONION_PI_-_REV_BR&edit-text=&act=url))，电池供电，连接 4G 网络。

[Jose]的 OnionPi 设置基于 [Adafruit 版本](https://learn.adafruit.com/onion-pi/overview)，但是增加了一些有趣的特性，使它更加有用。它由电池供电，充电时间约为一天，内置电池充电器，以太网直通，外部 4G 和 WiFi 天线，所有这些都在一个密封的外壳中，使整个建筑不受元素的影响。

虽然这本身算不上什么黑客，但集成的数量令人印象深刻。有开关可以关闭每个单独的网络端口，所有相关的插头都连接到前面板，交流输入和 USB 串行连接使用螺丝连接器，据说这在巴西非常流行。

[Jose]还带来了一个新设备，这个设备在网上其他地方都没有记载。它被称为 NNCFA，或无新密码。使用一个有趣的带有 SATA 连接器的 ARM 单板计算机，Jose 创建了一个可以在硬盘上安装 TrueCrypt 卷并通过 Samba 共享它们的设备。