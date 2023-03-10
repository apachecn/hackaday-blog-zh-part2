# Arduino 云。云就是云的意思。

> 原文：<https://hackaday.com/2013/09/12/the-arduino-yun-yun-means-cloud/>

长久以来，Arduino 的创造者一直在考虑如何将 Arduino 平台引入云中。以太网和 WiFi 屏蔽在技术上是可行的，但是如果你正在处理从网页上抓取的数据，一个低级的微控制器真的不是最好的选择。进入 [Arduino 云](http://blog.arduino.cc/2013/05/18/welcome-arduino-yun-the-first-member-of-a-series-of-wifi-products-combining-arduino-with-linux/)。在它的核心，它是一个普通的老 Arduino 莱昂纳多。在木板上的金属板下面？那是一个运行 Linux 的 SoC。

基本上，云的 Linux 端非常类似于运行 OpenWRT 的 WiFi 路由器。有一个 USB 端口用于插入外围设备，原生 WiFi 支持(802.11n，甚至！)，一个以太网连接器，以及足够的 RAM 来做所有连接到互联网的小型计算机可以做的有趣的事情。

为了让 Arduino 新手更容易进行所有这些 web 编程，YUN 还包括一个“桥”库，可以自动化 YUN 的 Linux 和微控制器端之间的 HTTP 事务。它还支持 Temboo T1，这是一个用于几十个 API 的 SDK，这些 API 与脸书、Dropbox、联邦快递和数百个其他网络服务进行交互。

下面你可以看看[Massimo]和[David]展示他们的产品，并了解云如何通过“桥”连接到互联网并与微控制器交互。这是一个有趣的装置，我们肯定会在世界创客大会上看到。

[https://www.youtube.com/embed/kwHVeWADs2Y?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/kwHVeWADs2Y?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)