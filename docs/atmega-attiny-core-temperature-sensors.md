# ATMega 和 ATtiny 核心温度传感器

> 原文：<https://hackaday.com/2014/02/01/atmega-attiny-core-temperature-sensors/>

![temp](img/bcf0f701de1148e36c0c9c3c44d04054.png)

我们不知道这是否会让普通黑客读者感到惊讶，但一大堆 Atmel 微控制器在其数据手册中隐藏了一个非常酷的功能。它们中的大多数——从 ATMega 168、328、32u4，到 ATtiny85 和 84，都在芯片上有一个温度传感器。[Connor]对这个传感器做了一点研究，[想出了一点代码](http://www.narkidae.com/research/atmega-core-temperature-sensor/)，它通过串行端口输出这些 Atmel 芯片的核心温度。

这些 Atmel 芯片上的温度传感器通过向芯片上的 ADMUX 寄存器写入一个代码来访问，例如 Mega32u4 为“100111 ”, tiny 84 为“100010”。根据数据表，返回的温度精确到+-10°C，但可以通过将一块冰块(当然是在塑料袋中)放在芯片上来轻松校准。

只需多一点代码，[Connor]就能通过串行端口输出微控制器内核的温度。在测试中，他的芯片从 20℃开始，大约一分钟后在 24℃达到平衡。非常简洁，必要时可以用作项目的温度传感器。