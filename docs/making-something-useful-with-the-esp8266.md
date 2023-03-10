# 用 ESP8266 做点有用的东西

> 原文：<https://hackaday.com/2015/01/05/making-something-useful-with-the-esp8266/>

ESP8266 是让项目连接到互联网的最新和最棒的方式，但迄今为止，我们还没有看到许多项目真正使用这种非常酷的芯片做一些事情。是的，有一些人在使用 AT 命令，有一个欣欣向荣的社区在这个芯片上构建解释器和闪烁新代码，但在实际项目中并不多见。[马丁]是个例外。他提出了两个使用 ESP8266 的项目。

第一个项目是把 DHT22 温度/湿度传感器的读数放到互联网上。遵循 ESP8266 所有最新开发的精神，[Martin]没有使用外部微控制器。相反，他使用 SDK 运行[一个使用【Sprite_TM】代码的 HTTP 守护进程](http://www.esp8266.com/viewtopic.php?f=6&t=376)。该网络服务器提供了一个开关 LED 的界面，并报告来自 DHT22 的温度和湿度读数。这很简单，但很容易看出这个小小的芯片如何成为智能恒温器的基础。

如果点亮 led 还不够的话，[Martin] [还有另一个项目，包括三个固态继电器](http://harizanov.com/2014/12/wifi-iot-3-channel-relay-board-with-mqtt-and-http-api-using-esp8266/)。这个稍微复杂一点，有 [MQTT 支持](http://en.wikipedia.org/wiki/MQTT)，一个花哨的 jQuery 接口，以及对网络时间的支持。[Martin]还没有准备好发布这个项目的完整代码，但那只是因为在公开之前他想实现一些功能。这些功能包括动态 DNS、计划功能和对 I2C 状态显示的支持。即使没有这些花哨的功能，它仍然是一个非常棒的项目，仍然非常适合物联网。您可以在下面查看[Martin]关于该板的视频演示。

[https://www.youtube.com/embed/SAswDqyTatY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/SAswDqyTatY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

谢谢你的提示。