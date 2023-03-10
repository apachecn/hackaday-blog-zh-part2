# 用 STM32F4 构建发动机控制单元

> 原文：<https://hackaday.com/2014/01/01/building-an-engine-control-unit-with-the-stm32f4/>

如果你想加大马力，首先你可能会看发动机控制单元。这台插在发动机舱里的电脑控制着你汽车性能的方方面面，从空气/燃料比，点火时间，到阀门控制。升级 ECU 通常意味着在设备上刷新新的固件，但[Andrey]更进一步:[他正在使用 STM32F4 发现开发板构建自己的 ECU](http://rusefi.com/) 。

[Andrey]的座驾是一辆 1996 年的福特 Aspire，但在他开发开源 ECU 时，他希望能够驾驶自己的汽车。没问题，就像去垃圾场，捡一个备用的，[和逆向工程，](http://rusefi.com/articles/stimulator/)是一种便宜又简单的开发方式。在用 ATX 电源为这个备用 ECU 供电后，[Andrey]能够设计出一个电路来将传感器输入到他的微控制器，并让他的开发板控制燃料喷射器。

[通过一些额外的硬件](http://rusefi.com/hardwave/)【Andrey】打开 ECU，控制燃油喷射、点火、燃油泵和怠速空气阀电磁阀。对于福特工程师花费数千工时创造的东西来说，这是一个不错的替代品。

[Andrey]的 ECU 实际上也能工作。在下面的视频中，你可以看到他驾驶着他的 DIY ECU 控制着发动机的各个方面，在一个被雪覆盖的废物周围行驶。如果发动机听起来有点粗糙，那是因为一根电线松了，他只使用了两个气缸。不过，一点热胶水就能解决这个问题。

[https://www.youtube.com/embed/NJSQV5utGXw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/NJSQV5utGXw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)