# 皮安范围的数据记录

> 原文：<https://hackaday.com/2015/08/26/data-logging-in-the-picoampere-range/>

您可能知道，要在电源和负载之间传输最多的能量，它们的阻抗需要匹配。这就是为什么业余无线电发射机需要一个 50 欧姆的天线(至少，通常是这样)。发射器是 50 欧姆，你想要一个匹配。一些测试设备匹配阻抗，但对于万用表、示波器和许多其他设备，仪器只是呈现非常大的阻抗。只要比被测电路的阻抗大很多，影响就很小。

对于当今的 MOSFET 仪表放大器，很高的输入阻抗并不罕见。然而，您有时会遇到输入 Z 值较低的情况，如果您不考虑这些情况，可能会导致问题。另一方面，一些人看到问题，另一些人看到机会。

[Paul Allen 的] SigZig 数据记录器就是一个很好的例子。它的输入 Z 约为 33 万欧姆。没有现代示波器或数字电压表那么高，但与你通常想要测量的相比还是相当高的。SigZig 的噪声系数非常低，因此 SigZig 的人员决定尝试利用 330K 输入 Z 来测量非常小的电流。

[![zig](img/1f365fc5726dff808605d72ee9d4e0fc.png)](https://hackaday.com/wp-content/uploads/2015/08/zig.jpg) 使用一些基本的数学模型，他们能够检测到 115 皮安的变化。右图显示了加载 1.25V 电源的 1 千兆欧电阻和 1.1 千兆欧电阻之间的差异。你可以看到有一点噪音，但信号清晰可辨。显然，如果没有低噪底，很难将信号从如此低的噪声中分离出来。但是正如我们之前提到的，西格非常安静。如果您需要提升阻抗，[我们也能满足您的需求](http://hackaday.com/2015/07/29/say-it-with-me-input-impedance/)。

[https://www.youtube.com/embed/t1AAZrStPvs?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/t1AAZrStPvs?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

via [ [危险原型](http://dangerousprototypes.com/2015/08/19/using-input-impedance-to-measure-current/)