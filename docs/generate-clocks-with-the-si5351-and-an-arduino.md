# 用 SI5351 和 Arduino 产生时钟

> 原文：<https://hackaday.com/2014/06/27/generate-clocks-with-the-si5351-and-an-arduino/>

如果处理 RF，可能需要产生各种时钟信号。幸运的是，[Jason]已经应用他的知识为 Arduino 构建了一个 SI5351 库和一个芯片分线板。

SI5351 是一款可编程时钟发生器。它最多可以输出 8 kHz 至 133 MHz 的 8 种独特频率。这使得它成为构建 RF 项目的便捷工具。[Jason]的分线板在 SMA 连接器上提供 3 个隔离时钟输出。一个插头连接到一个 Arduino 上，Arduino 为 I2C 提供电源和控制。

如果你正在寻找一种应用，[Jason]的原型单边带无线电展示了芯片的作用。这台收音机使用两个 SI5351 时钟:一个用于 [VFO](http://en.wikipedia.org/wiki/Variable-frequency_oscillator) ，一个用于 [BFO](http://en.wikipedia.org/wiki/Beat_frequency_oscillator) 。这减少了器件数量，使这种设计非常便宜。

Arduino 库[可以在 Github](https://github.com/etherkit/Si5351Arduino) 上获得，你可以[从 OSHPark 订购 SI5351 分线板](https://oshpark.com/shared_projects/abfFTk0x)。