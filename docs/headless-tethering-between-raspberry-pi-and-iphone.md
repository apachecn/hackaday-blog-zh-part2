# Raspberry Pi 和 IPhone 之间的无头共享

> 原文：<https://hackaday.com/2013/07/29/headless-tethering-between-raspberry-pi-and-iphone/>

![rpi-iphone-tethering](img/b23fc314ddcc7de5ad6a5ccba1369bf8.png)

这个黑客不一定有目标应用程序。但是有很大的潜力。这是一个无头的设置，用于将你的树莓派与 iPhone 绑定。立即想到的是建立上传到互联网的传感器阵列(实时或只是转储其日志)。但是我们确信还有很多其他的应用等着我们去想。

使用树莓 Pi 进行共享非常简单。只需安装存储库中可用的几个包，并快速调整配置文件以允许热插拔。但是这依赖于安装的 iPhone，并且该任务通常只有在 GUI 运行时才是自动的。为了不使用 X desktop ,[ Dave Controy]通过 ifuse 设置从命令行安装手机。结果是，只要 iPhone 插入，您的 RPi 就会建立网络连接，无需您的任何干预。

[谢谢迈克尔]