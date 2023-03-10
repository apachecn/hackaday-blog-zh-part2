# Arduino SPI 库获得事务支持

> 原文：<https://hackaday.com/2014/08/01/arduino-spi-library-gains-transaction-support/>

![Transaction SPI Timing](img/a06dec10310a8d44dc34e7bbedeef099.png)

Transaction SPI Timing

在同一总线上使用多个 SPI 器件时，为了防止数据损坏，必须注意确保只能从主环路内部或中断例程访问这些器件，而不能同时从两者访问。当一个器件在主环路中被片选，然后在传输过程中发生中断，片选另一个器件时，可能会发生数据损坏。原始设备现在获得不正确的数据。

在过去的几周里，[Paul]一直在开发一个新的 [Arduino SPI 库](http://www.dorkbotpdx.org/blog/paul/spi_transactions_in_arduino)，以解决这些类型的冲突。在上述场景中，新库将生成一个阻塞 SPI 事务，从而允许第一个主循环 SPI 传输在尝试第二个传输之前完成。如上图所示，蓝色走线上升沿是在绿色走线片选期间发生中断的时间。最好的部分，它只影响 SPI，你的其他中断仍然会按时发生。没有伺服抖动！

这只是图书馆的新功能之一，其余的请点击上面的链接。[Paul]总结得很好:“保护您的 SPI 访问不受其他基于中断的库的影响，并保证在您使用 SPI 总线时设置正确”。