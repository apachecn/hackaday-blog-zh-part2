# 新零件日:ESP8266 黑仔

> 原文：<https://hackaday.com/2015/07/13/new-part-day-the-esp8266-killer/>

大约在去年的这个时候，我们第一次听说了 ESP8266 WiFi 模块。它仍然是一个很棒的小模块，为所有这些物联网事物提供 WiFi 连接，价格仅为 5 美元。对于一个巨大的模块来说，这是一个有吸引力的价格，一个巨大的社区为这个平台提供了很多项目。

现在街区里有了一个新成员。它被称为 EMW3165，像 ESP 一样，它为一系列无线项目提供 WiFi 连接。它拥有 STM32F4 ARM Coretex M4 微控制器、一个“自托管”网络库、更多 RAM、更多闪存和更多 GPIOs，功能更加强大。你可能会问自己。比 ESP8266 贵一美元。

模块的数据表介绍了所有的细节。虽然这款芯片有 3.6V I/o，但也有一些 5V 兼容引脚——这对 Arduino 人群来说是一个福音。对于连接到 802.11n 网络的东西来说，这也是令人惊讶的低功耗。这里真正的好处是 STM32F4 内核——这是一个非常非常强大的微控制器，如果你想要一个 2 组件 WiFi 网络摄像头，这是你应该使用的部分。使用这部分将会有很多有趣的构建。[也通过了 FCC 认证](https://hackaday.com/wp-content/uploads/2015/07/fccid-io-2551077.pdf)。非常酷。