# 逆向工程 ST-Link/V2 固件

> 原文：<https://hackaday.com/2013/01/07/reverse-engineering-st-linkv2-firmware/>

![reverse-engineering-stlink-v2](img/8949dcd619e661fe6d80a6d246a579bb.png)

这张图片中央上方的芯片是手臂皮层-M3。它能够对 STM32F3 发现板上的主芯片进行接口和编程。使用的协议是 ST-Link/V2，它已经成为 ST 微电子开发板的标准。问题是，图像底部附近的大 ARM 芯片有多个 UARTs，桥接几个焊点会将其连接到 ST-Link 硬件。[Taylor Killian]想要弄清楚是否有内置固件支持来使其成为 USB 转串行转换器，他的解决方案涉及到对 ST-Link/V2 固件进行逆向工程。

挑战的第一部分是获得固件映像。当您下载固件更新包时，映像并不作为独立文件包含在内。相反，他必须在固件更新期间嗅探 USB 流量。他设法分离出文件，并找到了正在使用的加密技术。这是一个有趣的阅读，看看他是如何做到这一点的，我们期待着了解他现在可以完成什么，得到他所追求的商品。