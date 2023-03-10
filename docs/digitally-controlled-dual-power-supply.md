# 数字控制双电源

> 原文：<https://hackaday.com/2013/12/11/digitally-controlled-dual-power-supply/>

[Kerry]开始为他的工作台制造一个数字控制双电源。他已经基于 [LM338 线性调节器](http://www.kerrywong.com/2012/04/30/5a-lab-power-supply-with-digital-readout/ "LM338 Linear Supply")构建了一个电源，但这次的目标是在没有线性调节器 IC 的情况下构建它，并添加对电流和电压的数字控制。

在制作的第一部分中，[Kerry]解释了设备的模拟设计。他有一个额外的散热器，可以从这个线性电源中散发足够的热量，使其在 10 A 下运行。一个 [NE5532](http://www.ti.com/lit/ds/symlink/ne5532.pdf) opamp 用于跟踪参考电压，该电压可以由 DAC 提供。电流由 [LT6105](http://cds.linear.com/docs/en/datasheet/6105fa.pdf) 分流检测放大器测量，然后与另一个 DAC 提供的参考进行比较。

[第二部分](http://www.kerrywong.com/2013/12/02/a-digitally-controlled-dual-tracking-power-supply-ii/)重点介绍数字元件。为了与模拟电路接口，使用了两个[MCP 4821](http://ww1.microchip.com/downloads/en/DeviceDoc/21953a.pdf)DAC。这些由 ATmega328P 通过 SPI 控制。

幸运的是，[克里]也有他自己的[DC 负载项目](http://hackaday.com/2013/10/28/building-a-dc-constant-currentpower-electric-load/ "Building a DC Constant Current/Power Electric Load")来测试供应。