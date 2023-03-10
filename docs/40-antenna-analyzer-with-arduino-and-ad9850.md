# 40 美元天线分析仪，集成 Arduino 和 AD9850

> 原文：<https://hackaday.com/2015/08/06/40-antenna-analyzer-with-arduino-and-ad9850/>

如果你是一名黑客，你可能会认为业余无线电爱好者是创新的。然而，大多数人只是认为它们很便宜。所以毫不奇怪，像[jmharvey]这样的火腿会从一个 DDS 模块和一个 Arduino 构建一个[天线分析器](https://github.com/jmharvey1/DDS_AD9850_AntennaAnalyzer)，而不是花几百美元购买一个商业单元。正如他所指出的，在安装天线的时候，你可能只需要一两天的分析器。除非你是一个一流的天线制造商，否则这个设备会闲置在货架上(或者会以比你更便宜的价格借给 hams)。

这个设计源于另一个成熟的设计，但是利用了他手头上的一些零件。虽然构建是在通用电路板上，但[jmharvey]使用 Eagle 来布局电路，就好像它是 PCB 一样。对于 RF 电路来说，位置很重要，所以这不是一个坏主意。在屏幕上移动东西总是比在性能板上更容易。

由于这是一个简单的单元，您应该从 Arduino 中获取输出，并手动将其放入电子表格中以绘制结果。有另一个版本的 Arduino 代码可以驱动有机发光二极管屏幕，尽管你仍然需要一台 PC 来启动这个过程。Arduino 代码的一个有趣特性是它如何处理电路中使用的二极管的非线性特性。在绘制了已知负载下的值后，[jmharvey]将二极管操作分为三个区域，并对每个区域使用不同的方程。即便如此，他警告说，高于 1:1 VSWR 的读数只精确到 10%或 20%——对于火腿小屋的使用来说仍然足够了。

如果你想要一个 40 美元(或者更少，如果你有一个好的零件库存)的天线分析仪，这看起来是一个值得的项目。然而，如果你想把它转用于你邻居的调幅收音机，你可能会选择商业单元。

单击休息处，查看分析器的运行情况。

[https://www.youtube.com/embed/C6YxD72sX_Y?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/C6YxD72sX_Y?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)