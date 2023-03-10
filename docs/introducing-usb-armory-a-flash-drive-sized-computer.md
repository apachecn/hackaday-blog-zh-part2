# 介绍 USB Armory，一种闪存盘大小的计算机

> 原文：<https://hackaday.com/2014/10/14/introducing-usb-armory-a-flash-drive-sized-computer/>

[Andrea]向我们透露了关于[USB armory](http://inversepath.com/usbarmory)的信息，这是一个用于安全项目的微型嵌入式平台。它基于 800 MHz ARM Cortex-A8 Freescale I . MX53 和 512 MB DDR 3 SDRAM，包括一个 microSD 卡插槽、一个带 gpio/UART 的 5 引脚分线接头、一个可定制的 LED，并通过 USB 供电。

这种特殊的处理器支持一些高级安全功能，如安全引导和 ARM TrustZone。安全引导功能允许用户融合验证密钥，以确保只有可信固件才能在主板上执行，而 ARM TrustZone 则在内存和外设级别强制执行“安全”和“正常”领域之间的域分离。这使得许多项目，如电子钱包，认证令牌和密码管理器。

完整的设计是开放的硬件，它的所有文件都可以从官方的 [GitHub 库](https://github.com/inversepath)下载。第一版最终设计的目标价格是€100 左右。