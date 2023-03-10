# 在不带传感器的 AVR 上测量温度

> 原文：<https://hackaday.com/2015/05/02/measuring-temperature-on-an-avr-without-a-sensor/>

有一些 AVR 微控制器带有板载温度传感器。这些温度传感器既不准确也不精确，但它们确实适用于一些用例。[Thomas] [想出了一点代码](https://hackaday.io/project/5534-avr-temperature-measurement-without-a-sensor)，它可以在所有 AVR 微控制器上运行，并且至少与拥有它们的罕见 AVR 中的传感器一样准确。

虽然并非所有 AVR 都有温度传感器，但它们都有 RC 振荡器，并且这些 RC 振荡器对温度敏感。通过结合 RC 振荡器和看门狗定时器，[托马斯]的代码可以得到一个模糊的想法，如果它变得更热或更冷。

为了证明他的代码有效，[托马斯]拿了一个加载了少量代码的 ATtiny13A 芯片，并在上面放了一枚加热的硬币。该芯片被编程为当它检测到温度上升时打开 LED，不出所料，LED 亮了。随着一枚硬币在一碗冰水中冷却，另一段代码运行，led 闪烁。

虽然我们肯定它既不准确也不精确，但它确实有它的用途——过热保护或简单的恒温器。您可以查看下面的代码运行视频。

[https://www.youtube.com/embed/NppARTy1Ga8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/NppARTy1Ga8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)