# 使用 NRF24L01 进行空气引导装载

> 原文：<https://hackaday.com/2014/03/07/using-an-nrf24l01-for-air-bootloading/>

![nrfboot_small](img/ce6643e026cb28e5a39ed810fce2d336.png)

[死灵]编写了一个库，使用 NRF24L01 无线通信模块，通过 RF 链接刷新他的微控制器。NRF 24l 01 是一款廉价的 RF 模块，可以轻松集成到许多微控制器项目中。尽管有驱动 NRF24L01 的 Arduino 库，[Necromat]决定开发一个没有 Arduino 依赖的端口。

由此产生的引导加载程序适合 ~~RAM~~ 闪存的 4K，具有数据包丢失和恢复功能，以及用户可配置的硬件或软件 SPI。编程速度不是最高的，但[ ~~Necromat~~ 死灵]认为这是 VUSB 的特性，而不是 NRF24L01 或目标微控制器的传输速率。

为了给目标 AVR 芯片编程，[ ~~Necromat~~ 死灵]使用了另一个 NRF24L01 模块，通过 USB 连接到他的 [uISP](https://github.com/uISP/uisp-schematics) 加密狗。使用[定制工具](https://github.com/nekromant/rf24boot/tree/master/rf24tool)与 uISP 接口，目标板可以按照与 avrdude 类似的方式进行编程。在他的 [GitHub 页面](https://github.com/nekromant/rf24boot)上查看 ISP 加密狗和 AVR 引导程序的代码。