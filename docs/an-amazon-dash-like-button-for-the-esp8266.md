# ESP8266 的亚马逊破折号按钮

> 原文：<https://hackaday.com/2015/05/13/an-amazon-dash-like-button-for-the-esp8266/>

亚马逊 Dash 按钮是一个很小的硬件，包含一个按钮、一个 WiFi 模块和一个漂亮、闪亮的公司标志。按下按钮，带有该标志的产品将被送到你家。至少是令人印象深刻的营销。有了像 ESP8266 这样的小型廉价 WiFi 模块，开发出亚马逊 Dash 克隆版只是时间问题。

[deqing]使用 ESP-12 模块、一个按钮、一个 3D 打印外壳和一对 AA 电池创建了一个 ESP8266 仪表盘按钮。从电子角度来说，这非常简单；按下按钮，ESP 将唤醒，请求一个 URL，并使自己回到睡眠状态。当你复制亚马逊 Dash 按钮的功能时，这就是你需要做的所有事情——服务器会处理剩下的事情。

为了配置 ESP8266，[dequng]正在使用 Android 的 [ESP-TOUCH 应用程序，在这个 ESP 按钮中设置新功能就像在按钮的 Flash 中放入一个 URL 一样简单。](https://github.com/EspressifApp/EsptouchForAndroid)

这不仅是一个具有数百种不同用途的伟大构建，而且也不是 ESP8266 的分线板。很高兴我们终于在现实世界中看到一些使用这种廉价 WiFi 芯片的构建。

显然，实际的 Dash 按钮包括认证，而这个按钮没有。我们最近看到了原始硬件的拆卸。不过，我们仍在等待对下订单时喷到互联网上的数据进行深入分析。