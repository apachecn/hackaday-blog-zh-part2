# CC3000 WiFi 驱动程序。网络微处理器

> 原文：<https://hackaday.com/2013/08/27/cc3000-wifi-driver-for-net-micros/>

![CC3000](img/3f434541c57fd46c4a5e0f2208a4b481.png)

Netduino 和其他。网络微板似乎没有得到太多的爱，但这并不意味着他们不能使用我们在一段时间内看到的最酷的芯片之一。【瓦尔基里】[为 TI 新出的 CC3000 一体机 WiFi 芯片](http://cc3000.codeplex.com/)写了一个驱动，给任何。一个非常小而且非常便宜的 WiFi 连接。

不久前，[Chris Magagna] [为 Arduino 创建了 TI CC3000 库](http://hackaday.com/2013/06/24/tis-cc3000-wifi-chip-gets-a-library/)。[瓦尔基里]看到那个帖子时从椅子上掉了下来，因为它意味着。NET Micro 设备(如 Netduino)最终可以使用这种设备。通过 TI Launchpad 和逻辑分析仪，[瓦尔基里]记录了所有 SPI 命令和响应，最终重建了整个库。

至于这在没有任何硬件的情况下有多有用，GHI Electronics 已经推出了 CC3000 Gadgeteer 模块。