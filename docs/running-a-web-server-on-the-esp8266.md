# 在 ESP8266 上运行 Web 服务器

> 原文：<https://hackaday.com/2014/11/15/running-a-web-server-on-the-esp8266/>

我们最近写了很多关于 ESP8266 的文章，但是人们一直在寻找这个廉价模块的更棒的用途。[Martin]认为使用带有外部微控制器的 ESP8266 有些过分，并决定[完全在带有内置 web 服务器的模块](http://harizanov.com/2014/11/esp8266-powered-web-server-led-control-dht22-temperaturehumidity-sensor-reading/)上实施他的项目。

[Martin]从[sprite_tm]开发的 [ESP8266 web 服务器固件](http://www.esp8266.com/viewtopic.php?f=6&t=376)开始。这个固件提供了一个基本的网络服务器，支持多个连接和模块上的简单 CGI 脚本。网络服务器固件为 CGI 脚本提供了大量的可能性。在 AP 模式下启动时，您甚至可以直接从浏览器将 ESP8266 连接到另一个接入点。

[Martin]决定在模块上连接一个 DHT22 温度/湿度传感器作为概念验证。他使用为 ESP8266 编写的 [DHT22 库](https://github.com/fasmide/esp_dht22)从传感器读取数据，并编写了一个 CGI 脚本来在网页上显示数据。[Martin]还添加了控制 GPIO 引脚的按钮作为概念验证。他发布了他的源代码和一个二进制文件(见他的帖子的结尾),所以你可以尝试他的应用程序并为你自己的项目修改它。