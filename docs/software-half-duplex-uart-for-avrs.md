# AVR 软件半双工 UART

> 原文：<https://hackaday.com/2014/01/13/software-half-duplex-uart-for-avrs/>

如果你在过去使用过非常低成本的微控制器，比如 AVR 的 ATtiny 系列，你可能会被没有 UART 外设所困扰。这个问题的通常答案是用软件实现 UART。速度不快，但很管用。

假设您的资源更加有限，只有一个 UART 引脚。[Ralph]创建了一个软件库和一个小电路，仅使用一个引脚就能实现[半双工 UART。有了上面的电路和一个 62 字节的 Arduino 兼容库，你可以把 UART 加到最小的 ATtinys 上。](http://nerdralph.blogspot.ca/2014/01/avr-half-duplex-software-uart.html)

在此电路中，Tx/Rx 引脚位于 AVR 上，Tx 和 Rx 引脚是另一个器件。该电路依赖于 UART 的空闲状态为逻辑高信号。当 Tx 引脚空闲时，晶体管保持导通。当 AVR 发送 0 时，Tx/Rx 引脚可以将 Rx 拉低。当 Tx 引脚发送 0 时，Tx/Rx 引脚通过二极管被拉低。

这是一个聪明的方法，绝对可以帮助你的下一个小项目增加交流。