# 面向 MSP430 的更好的 USI I2C 图书馆

> 原文：<https://hackaday.com/2014/02/02/a-better-usi-i2c-library-for-the-msp430/>

![USI](img/9c3ec838c1a76988d53c55d999b9460d.png)

TI 的 MSP430 芯片相当有趣——它们功耗低，功能强大，大多数情况下售价不到一美元。不过，其中一些芯片没有本地 SPI 或 I2C 接口；相反，一切都是通过 USI 或通用串行接口模块完成的。[Jan]发现股票 I2C USI 模块有点粗糙，[所以他创建了自己的](http://jan.rychter.com/enblog/msp430-i2c-usi-library-released)。

[Jan]发现 TI 将 USI 用作 I2C 设备的示例代码过于复杂，而且是一名实习生在一周内完成的，之后就再也没有接触过。作为回应，他创造了一个非常非常简单的 USI/I2C 模块，实际上是可读的。如果你想自己拿的话，可以在 GitHub 上找到。

与 TI 代码相比，【Jan】的库非常简单。只有两个函数，一个用于初始化，另一个用于发送和接收。简单，小巧，而且有效。没有比这更好的了。