# 用于 ESP8266 WiFi 芯片的 SDK

> 原文：<https://hackaday.com/2014/10/25/an-sdk-for-the-esp8266-wifi-chip/>

ESP8266 是一款最近吸引了很多人的芯片，它将 WiFi 无线电、TCP/IP 堆栈和互联网上的微控制器所需的所有比特都塞进了一个 5 美元的小模块中。这是一个有趣的芯片，不仅因为它是一个 UART 到 WiFi 模块，允许几乎所有的东西以 5 美元的价格上网，而且因为在这个板上有一个用户可编程的微控制器。如果我们有一个 SDK 或几个库就好了…

[ESP8266 SDK 终于来了](http://bbs.espressif.com/viewforum.php?f=5)。一个完整的用于 ESP8266 的 SDK 刚刚被发布到 Expressif 论坛，[以及一个带有 Ubuntu 的 VirtualBox 映像](http://bbs.espressif.com/viewtopic.php?f=5&t=2)，该映像包括用于该模块的 LX106 内核的 GCC。

SDK 中包括 SSL、JSON 和 lwIP 库的源代码，这使得它成为您需要使用物联网做的几乎所有事情的解决方案。就 LX106 内核而言，有使用该板上的备用引脚作为 GPIOs、I2C 和 SPI 总线以及 UART 的示例代码。

这使 ESP8266 成为比 UART 转 WiFi 模块好得多的东西；现在你只需要 5 美元的硬件就可以创建一个物联网。我们很想看到一些例子，所以把它们放在 [hackaday.io](http://hackaday.io/) 上，发送到举报热线。