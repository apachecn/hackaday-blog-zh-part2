# ESP8266 WiFi 投掷器

> 原文：<https://hackaday.com/2015/05/03/esp8266-wifi-throwies/>

几年前，有人发现你可以把一个 LED、一个硬币电池和一块磁铁粘在一起，然后把它们扔在任何可以想象的金属表面上。这是发光二极管的发明，世界因为它的发明而变得更加糟糕。

有了 ESP-8266 WiFi 模块，我们就有了一个带 WiFi 无线电的微型*微型*设备，以及足够做一些有趣事情的处理能力。那是什么意思？ [WiFi 投掷](https://www.youtube.com/watch?v=fQM-GHY6VJ8)。

[Andreas Reischle]将一个 ESP-8266 WiFi 模块和一个锂电池塞进一个装有磁铁的防风雨控制器中。就其本身而言，这些不会做太多，但通过正确的软件组合，这个小磁盒可以作为一个接入点，为任何连接的人提供小型 JavaScript 游戏。

该软件基于 [NodeMCU 固件](https://github.com/nodemcu/nodemcu-firmware)，并具有网络服务器和 DNS 服务器。web 服务器的效用是显而易见的，DNS 服务器将所有流量重定向到设备的 index.html 文件，在那里显示一个小 JavaScript 游戏菜单。

比用 led 和锂污染世界好多了；这个上面有 Hunt Wumpus。

谢谢[奥利弗]的提示。

[https://www.youtube.com/embed/fQM-GHY6VJ8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/fQM-GHY6VJ8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)