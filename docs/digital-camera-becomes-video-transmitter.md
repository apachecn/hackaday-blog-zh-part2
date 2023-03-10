# 数码相机成为视频发射器

> 原文：<https://hackaday.com/2013/09/12/digital-camera-becomes-video-transmitter/>

![canon](img/d6fb9965e3dd91db2c6995c3d087275a.png)

在高空气球领域，佳能的 PowerShot 系列数码相机是将气球送入平流层的热门相机。这有一个特殊的原因:这些相机可以运行非常强大的 CHDK 固件，将一个 100 美元的数码相机变成一个内置 intervalometer 的相机，以及一系列非常酷的功能。似乎这个 CHDK 固件比我们想象的要强大得多，因为[Chris] [现在正在将佳能 a530 拍摄的照片传输到地面](http://chris-stubbs.co.uk/wp/?p=375)，只使用了 CHDK 固件和一个廉价的无线电模块。

这些 PowerShot 相机内部有一个运行 VxWorks 的 ARM 处理器，VxWorks 是一个最小但非常强大的嵌入式设备和火星探测器操作系统。通过连接相机的 Tx 和 Rx 线，[Chris]可以向操作系统发出命令，更改设置，甚至安装自己的代码。

在[Phil Heron]用 C 语言编写的 SSDV 编码器的帮助下，[Chris]能够让相机通过一个安装在电池盒中的小型无线电发射器传输图像[。现在，[克里斯]只为佳能 a530 建造了 CHDK + SSDV，但鉴于这种建造是如此有用，我们预计很快就会看到改进的版本。](http://www.radiometrix.com/node/343)