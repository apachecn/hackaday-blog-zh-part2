# 移位寄存器和多路复用器发光二极管的实验

> 原文：<https://hackaday.com/2015/03/18/an-experiment-in-shift-registers-and-multiplexed-leds/>

[Kratz]正在研究一种由 WiFi 控制的记分牌，但在建造全尺寸版本之前，他认为测试显示器的多路复用技术是明智的。[实验成功了](http://burnt-traces.com/?p=394)，但是除非这个记分牌是用来做桌上足球的，否则他还有很多工作要做。

这种原型显示器的设计非常简单，只有两个 595 移位寄存器向显示器提供位。十六个 NPN 晶体管用于吸收和提供电流给显示器。这是一个相对简单的电路，允许[Kratz]在一个小电路板上安装九个七段显示器，仅用六根线连接微控制器，包括地线、逻辑和 led 的两个 V+、时钟、数据和锁存器。

设计中有一些小问题:数据在上升沿读入，但锁存前需要额外的下降沿。[Kratz]找不出原因，这可能只是一个时间问题。