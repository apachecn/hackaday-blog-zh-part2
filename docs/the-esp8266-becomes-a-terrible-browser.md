# ESP8266 变成了一个可怕的浏览器

> 原文：<https://hackaday.com/2014/10/04/the-esp8266-becomes-a-terrible-browser/>

ESP8266 正在从中国来到世界各地的修理者的工作台上，用于令人惊讶的网络闪烁 led 项目等。[TM]认为他可以用他的 WiFi 到 UART 模块[做一些更酷的事情，并决定将一个模块变成网络浏览器](http://hackaday.io/project/3072-esp8266-retro-browser)。

ESP8266 上没有运行新的代码——所有的 HTML 都通过 Arduino Mega 推送，从服务器请求数据(在本例中是[我们神话般的复古版](http://retro.hackaday.com/))，并将数据发送到 Arduino 串行控制台。首先用几个 AT 命令向 ESP 模块发起连接，然后连接到 retro 服务器，最后将收到的所有内容转储到控制台。

并不多——HTML 标签仍然显示，图像当然是不可能的。然而，结果和你从 Lynx 得到的并没有太大的不同，这意味着这个古老浏览器的 Arduino 端口面临着挑战。