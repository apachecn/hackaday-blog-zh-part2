# Micro Python 现在在 ESP8266 上运行——贡献者希望让 Wifi 正常工作

> 原文：<https://hackaday.com/2014/11/29/micro-python-now-runs-on-the-esp8266-contributors-wanted-to-get-wifi-working/>

[Damien]给我们发了一封简短的电子邮件，告诉我们 Micro Python 是 Python 脚本语言在微控制器上的一种精简而快速的实现，现在运行在 ESP8266 上。你可能还记得[在 Hackaday 上对他的采访](http://hackaday.com/2013/11/27/interview-with-damien-george-creator-of-the-micro-python-project/)，那时微 Python 还处于众筹阶段。他的竞选筹集了 97k(目标是 15k ),它的评论部分让我们知道支持者对他的表现非常满意。

由于非常便宜的 ESP8266 Wifi 模块引起了很多关注，他实现了对它的支持。您可以使用[主存储库 ESP8266 文件夹](https://github.com/micropython/micropython/tree/master/esp8266)中的专用文件和 [esp-open-sdk](https://github.com/pfalcon/esp-open-sdk) 或者简单地使用预编译的二进制文件[这里](http://micropython.org/resources/upy.img)。不幸的是，该软件还没有 WiFi 支持，因为它目前只是一个通过 UART 的 Python REPL 提示符。因此，欢迎贡献者帮助加快开发速度！