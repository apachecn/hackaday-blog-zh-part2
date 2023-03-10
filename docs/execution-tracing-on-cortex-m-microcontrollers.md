# M3 微控制器上的执行跟踪

> 原文：<https://hackaday.com/2015/03/09/execution-tracing-on-cortex-m-microcontrollers/>

如你所料，更高功率的 ARM 微处理器有一堆用于程序和数据跟踪的调试工具。这一特性——CoreSight Trace 宏单元——也存在于低端 ARM Cortex M3 微控制器中。Cortex M3 正在许多项目中找到自己的路,[Petteri]想知道为什么这些调试工具看起来不够频繁。是缺少工具还是缺少文档？现在这已经不重要了，[因为他知道如何用一个便宜的逻辑分析仪和一些跟踪信号的解码器来完成。](http://essentialscrap.com/tips/arm_trace/)

在大多数 M3 皮层芯片中有两个轨迹块:ITM 和 ETM。仪器跟踪宏单元是跟踪观察点和中断这两者中的较高级别。嵌入式跟踪宏单元显示 CPU 中执行的每一条指令。这两者都可以用廉价的基于 FX2 的逻辑分析仪读取，这种分析仪可以通过通常的插座找到，价格约为 10 美元。然后问题就变成了软件，[【pet Teri】为此写了几个解码器](http://www.sigrok.org/blog/new-protocol-decoders-arm-tpiu-itm-etmv3)。

为了展示调试能力，[Petteri] [在他选择的 CNC 控制器 Smoothieboard 中找到了一个 bug](http://essentialscrap.com/tips/arm_trace/smoothie.html) 。偶尔，机器会漏掉一步。在跟踪工具的帮助下，通过对微处理器的欠锁，[Petteri]发现了挤压机舍入误差形式的缺陷。既然他知道了问题是什么，他就能想出解决问题的方法。他还没想明白。尽管如此，知道要修复什么是无价的，这是用普通工具无法找到的。