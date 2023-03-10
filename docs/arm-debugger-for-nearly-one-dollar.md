# 将近一美元的 ARM 调试器

> 原文：<https://hackaday.com/2014/01/23/arm-debugger-for-nearly-one-dollar/>

![](img/b78947befb3c4567ad195d1321b17344.png)

哦，这个标题太误导人了。但是如果你眯着眼睛挠头，这几乎是真的。多亏了[Peter Lawrence]的辛勤工作，现在有可能拼凑出一个极其便宜的 CMSIS-DAP ARM 调试器。

先说功能，回头再说成本。CMSIS-DAP 是一种标准，它为您提供了一种您期望从适当的调试器中获得的断点控制。在这种情况下,[Peter]在 PIC 16F1454 上使用 4k 字的空间实现了标准。这使它能够与 ARM 芯片上的调试端口对话，引导加载程序([也是他写的](https://code.google.com/p/pic16f1454-bootloader/))兼作 USB 到 UART 的桥梁。嘣，搞定。OpenOCD(和一些其他软件包)与 PIC 对话，PIC 与 ARM 对话。很好。

回到成本问题。量大的话近一块钱就能得到一个 16F1454。如果你切断一根旧的 USB 电缆，回收一些跳线，并且手头已经有电源和去耦，你就可以花将近 1 美元做生意了。