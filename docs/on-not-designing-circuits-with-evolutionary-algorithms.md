# 不使用进化算法设计电路

> 原文：<https://hackaday.com/2012/07/09/on-not-designing-circuits-with-evolutionary-algorithms/>

![](img/ec75bfee69300e4308d93e21d4f70e8f.png "animation")

[Henrik]一直致力于一个使用进化算法设计电子电路的程序。这仍然是一项进行中的工作，但他已经在 78 代(9 分钟的计算时间)后生成了一个像样的 BJT 反相器，如。以上 gif。

为了改进这些电路，[Henrik]告诉 SPICE 模拟生成一个具有 5V 电源、2N3904 和 2N3906 晶体管以及任何所需电阻的反相器。前十几代实际上没有做任何事情，但是在 2000 代之后，该算法产生了一个几乎与你在电路教科书中找到的 CMOS 反相器描述相同的电路。

用进化来指导电子设计并不是什么新鲜事；一个[进化算法和几个比特的 Verilog](http://www.damninteresting.com/on-the-origin-of-circuits/) 可以把一个 FPGA 变成一个芯片，这个芯片可以[以极低的硬件要求区分 1kHz 和 10kHz 的音调](http://www.amazon.com/Hardware-Evolution-Reconfigurable-Distinguished-Dissertations/dp/3540762531)。这个实验中还发生了一些非常非常奇怪的事情。进化算法利用了人类不可能编程的东西，并依赖于 FPGA 内部的磁通量和量子奇异性。

[Henrik]说他的算法没有测试有多少电流流过晶体管，所以在模拟之外实现这个电路会破坏晶体管并发出一股蓝烟。如果你想用进化来设计自己的电路，[Henrik] [把所有的代码放在 git](https://github.com/Ttl/evolutionary-circuits) 里供你阅读。它现在看起来很酷，一旦[Henrik]包括检查每个组件中的电流和电压，他的项目实际上可能是有用的。