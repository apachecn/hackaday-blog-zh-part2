# 用 Arduino 拯救 SD 卡

> 原文：<https://hackaday.com/2013/08/19/rescuing-an-sd-card-with-an-arduino/>

几天前，[Severin]的一个 SD 卡死了，他没有扔掉它，而是决定调查它到底出了什么问题，[最终使用 Arduino 和巨大的聪明恢复了大部分数据](http://tech.tiefpunkt.com/2013/08/sd-card-recovery-using-an-arduino/)。

SD 卡可以通过两种模式访问。第一种是 SDIO 模式，这是相机、笔记本电脑和其他读卡器使用的模式。第二种模式是 SPI 模式。SPI 比较慢，但是简单得多。结果是[Severin]卡上的 SDIO 模式被破坏了，但用 Arduino 和 SPI 模式访问它是有效的。终于有希望从这张损坏的卡上获取文件了。

[Severin]用一些草图把 SD 卡上的数据转储到他的电脑上。第一个查看了文件系统，并获取了卡上包含的文件列表。第二个遍历文件系统，并通过串行端口以十六进制输出所有文件。借助一点 Python，[Severin]能够重建一些以前永远丢失的文件。

即使 SD 卡完全无法用普通读卡器读取，[Severin]也能从卡上获取一些文件。所有的草图和 Python 脚本都可以在 Githubs 上找到[，随时可以从你损坏的 SD 卡上恢复文件。](https://github.com/tiefpunkt/arduino_sd_recovery)