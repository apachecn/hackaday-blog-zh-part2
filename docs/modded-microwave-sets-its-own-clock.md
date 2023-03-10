# 改进型微波炉设置自己的时钟

> 原文：<https://hackaday.com/2015/04/09/modded-microwave-sets-its-own-clock/>

在你家里所有的电器中，也许最令人讨厌的是一个带有闪烁的未设置时钟的微波炉。尽管现在很多设备都是自动设置时间的，但是大多数设备都需要在拔掉电源或者断电后设置时间。[Tiago]为了节省一点电能，他在工作时会关闭一些电器的电源，每次他插上微波炉的电源时，他都必须手动重置时钟。

谢天谢地[ 蒂亚戈写下了他对这个问题的解决方案:给他的微波炉添加一个附件，[通过网络自动设置时间](https://www.youtube.com/watch?v=aDWZkIIUHZk)。[Tiago]的项目使用运行我们之前介绍过的基于 [Lua 的固件](http://hackaday.com/2014/11/23/using-the-esp8266-as-a-web-enabled-sensor/)的 ESP8266。ESP 模块连接到[Tiago]的 WiFi 网络，并从他的 Linux 服务器上获取当前时间。

接下来，[蒂亚戈]拆开了他的微波炉，并在“设置时间”按钮和微波炉旋转编码器的两个输出引脚上钉了一些电线。为了安全起见，他让所有三个信号通过光隔离器，然后将它们路由到 ESP 模块上的几个 GPIO 引脚。当微波炉和 ESP 模块通电时，[Tiago]的 Lua 脚本从其服务器中获取时间，模拟按下“设置时间”按钮，并模拟旋转编码器输出来设置微波炉的时间。

虽然[蒂亚戈]没有发布任何关于他的构建的详细信息，但这看起来是一个很好的想法，可以很容易地加以改进(如添加 NTP 支持)。休息之后，请观看视频，了解实际设置。

[https://www.youtube.com/embed/aDWZkIIUHZk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/aDWZkIIUHZk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)