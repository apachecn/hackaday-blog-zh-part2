# PC 和 MCU 之间的 12 Mbps 通信

> 原文：<https://hackaday.com/2014/12/09/12-mbps-communication-between-a-pc-and-mcu/>

爱好电子产品的世界在过去几年才开始将 USB 应用到项目中，现在，在大多数情况下，将 1.5 Mbps 的速度推下 USB 端口已经足够了。这并不适用于所有情况；这是一个可怕的数据速率，真的，为了充分利用 USB 连接，[你至少可以移动到 USB 全速和 12 Mbps](http://hackaday.io/project/3579-12-mbps-communication-link-between-pc-and-mcu) 。

[Linas]在本例中使用了 STM32F4 微控制器，这是一款非常大且功能非常强大的芯片。[Linas]正在使用 FTDI 的 FT2232D USB UART 通过 USB 从 SPI 端口发送数据。这款芯片确实支持 12 Mbps，但只是在少量添加之后；外部 EEPROM 必须连接到 FTDI 芯片，以提供 USB 2.0 设备描述符，否则微控制器和计算机之间的连接速度将被限制在 1.5 Mbps。在这种情况下，即使在 STM32 上使用 USB 也是一个瓶颈；[Linas]仅使用 DMA 控制器将数据移出处理器——在 STM32 上使用 USB 会耗尽微控制器中的处理器周期。

由于 STM32 内部的 DMA 控制器，微控制器能够同时通过 SPI 发送和接收数据。STM32 能够同时读取和写入 Tx 和 Rx 缓冲区，但计算机只能进行半双工操作——它一次只能读取*或*写入。[Linas]正在将 STM32 上的 DMA 控制器设置为循环模式，将缓冲区中的所有内容放入 FTDI 芯片，并将计算机发送的所有内容读回到 STM32 的内存中。在数出正确的包数后。控制器重置所有内容，将循环缓冲区移回起点，并重新开始整个过程。

该电路的原型是一个 STM 发现板。借助 Labview，[Linas]可以看到来自微控制器的位，并通过 USB 将一些位发送回微控制器。[Linas]有一个关于这个项目的非常详细的视频教程。你可以看看下面。

[https://www.youtube.com/embed/JArPHfvhkCQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/JArPHfvhkCQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)