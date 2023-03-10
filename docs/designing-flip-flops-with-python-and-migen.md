# 用 Python 和 Migen 设计触发器

> 原文：<https://hackaday.com/2014/01/29/designing-flip-flops-with-python-and-migen/>

![migen](img/0693df8674c44677fe9984697c540cfa.png)

触发器是极其简单的电子电路，构成了时钟电路、存储电路、缓冲器和移位寄存器的基础。通过对数字逻辑的磨蹭，[杰弗里]决定建立自己的数字逻辑。不是用 Verilog 或 VHDL，而是 Migen:用软件构建数字电路的基于 Python 的方法。

Migen 是一个有趣的工具，它让传统的 FPGA 编程变得更加容易；Migen 允许用 Python 对 FPGA 编程，而不是 Verilog 或 VHDL。是的，这是你一直在等待的工具，[教程让它看起来很容易](http://milkymist.org/3/migen-tutorial.pdf)。在安装了 [Migen](http://jeffrey.co.in/blog/2014/01/installing-migen/) 之后，【杰夫】只用了三行代码就写了一个 D 触发器的类。那是三*可读的*行代码，他能够在另外两行代码中用 gtkwave 模拟触发器。与学习 VHDL 或 Verilog 的复杂性相比，Migen 使数字逻辑和 FPGA 编程变得轻而易举。

[Jeff]有一个很棒的关于用 Migen 构建 D 触发器的教程，但是我们希望看到一些更复杂的例子，看看这个非常酷的工具能做些什么。如果你正在用 Migen 制作(或已经制作)一些东西，请务必[发送到](http://hackaday.com/contact-hack-a-day/)并讲述你的经历。