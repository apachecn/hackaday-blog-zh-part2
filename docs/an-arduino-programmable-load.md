# Arduino 可编程负载

> 原文：<https://hackaday.com/2014/02/24/an-arduino-programmable-load/>

如果你在测试电池、电源、高功率 led、电镀或其他任何通常需要大电阻的东西，有一个大块的热电阻来倾倒电流是非常有用的。[Jakub]发现自己需要一个电子负载，而不是一个晶体管和一个罐子，决定做一些更自动化的东西:[一个围绕 Arduino 屏蔽建立的可编程负载。](http://kaktuscircuits.blogspot.cz/2014/02/mightywatt-arduino-electronic-load.html)

这种负载背后的想法非常简单:将一个器件连接到一个 FET 和分流电阻来测量电流。用运算放大器驱动 FET 的栅极，使其保持恒定电流或恒定电压。用一个 DAC 控制一切，你就有了一个由 Arduino 控制的可编程负载。

在如此小的外形下，散热肯定是个问题。为此，[Jakub]使用了一个 50×50 mm BGA 型散热器和一个 5V 风扇。如果它对一个大 CPU 来说足够好，它应该能够处理向 FET 倾倒 70 瓦的功率。还有一种保守的导热膏应用，在 FET 下面有一个非常小的热敏电阻，可以被 Arduino 读取。它可能会慢慢加热你的房间，但它不会着火。

有了 Arduino 草图[Jakub]为他的负载写的草图，他能够描述一对 Idea 电池的特性，并计算出三年前的可回收电池的电量。这是一项伟大的工作，如果[Jakub]愿意经历 Kickstarter 的麻烦，它将成为一个优秀的众筹产品。