# 6502 溢出是如何工作的

> 原文：<https://hackaday.com/2013/01/15/how-6502-overflow-works/>

[![6502 Overflow Circuit](img/fcda0e3276e288afed3e80004b0cdf49.png)](http://hackaday.com/2013/01/15/how-6502-overflow-works/6502overflow/)

6502 在 80 年代是一种无处不在的微处理器，为 Apple II 和任天堂娱乐系统等设备提供动力。[Ken]深入查看了处理器的一小部分:[溢出电路](http://www.arcfn.com/2013/01/a-small-part-of-6502-chip-explained.html "(A small part of) The 6502 chip explained down to the silicon")。

为了进行带符号计算，微处理器的算术逻辑单元(ALU)需要能够在溢出发生时进行计算。当两个数字相加后无法容纳在一个字节中时，就会发生这种情况。计算的结果将是不正确的，因此处理器必须通知程序发生了溢出。这是通过设置溢出标志来实现的。

【Ken】用这个例子首先解释溢出电路在逻辑上是如何工作的。然后他看了看门和逻辑的晶体管实现。最后，他向我们展示了实际 6502 芯片上的电路，展示了电路是如何在硅片上构建的。

这是一个很好的例子，可以让你多了解一些 alu 的工作原理以及集成电路是如何构建的。