# DIY 高稳定性时基黑客约 25 美元。为什么？频率稳定性很重要！

> 原文：<https://hackaday.com/2013/09/23/diy-high-stability-timebase-hack-for-25-why-frequency-stability-matters/>

[![DIY High Stability Timebase OCXO](img/4d0df8d7ec62d5775c0ff42f0bd3026d.png)](http://hackaday.com/wp-content/uploads/2013/09/diy-high-stability-timebase-ocxo.jpg)

如果你有一个旧的“Racal-Dana 199x”频率计数器或类似的 10 MHz 内部参考齿轮，具有较差的容差“标准石英晶体振荡器”或稍好的“温度补偿晶体振荡器”(TCXO)，你可以升级到一个高稳定性时基“恒温晶体振荡器”(OCXO)，价格不到 25 美元。[Gerry Sweeney]分享了他为自己的 Racal-Dana 频率计数器制作的 [DIY OCXO 电路](http://gerrysweeney.com/racal-dana-199x-diy-high-stability-diy-timebase-hack-for-under-25/)的设计和制作说明。我们已经看到[Gerry]对他的 HP 53151 a 进行了类似于[的升级，但是，这个电路更通用，可以捆绑在一小块可焊接的 perf 板上。](http://hackaday.com/2013/08/26/making-a-hp-frequency-counter-more-accurate/)

恒温振荡器使晶体保持稳定的温度，从而提高频率稳定性。根据您的起点，增加一个 OCXO 可以将您的频率容差提高 1 到 3 个数量级。当然，这不如我们过去见过的[铷频标构建](http://hackaday.com/2013/08/05/turning-a-rubidium-standard-into-a-proper-tool/)好，但正如[Gerry]所说，有一个不需要插入他的铷频标的便携式独立频率计数器是很好的。

[Gerry 的] [说明、原理图和数据表](http://gerrysweeney.com/racal-dana-199x-diy-high-stability-diy-timebase-hack-for-under-25/)可用于升级任何依赖于简单 10 MHz 基准(晶体或 TXCO)的实验室设备。他花了大约 20 美元在易贝买下了 OCXO——它可能很旧了，但我们确信随着时间的推移，它们会变得更加稳定。许多 OCXO 要求 5 V、12 V 或 24 V，因此您的设备需要适应正确的电压和电流负载。为了校准 OCXO，您需要一个温度稳定的可变电压基准，可以在 1 到 4 伏之间调节。他手头的 MAX6198A 符合 5 ppm/°C 温度系数的要求。同样重要的是，将基准电压源和调整电位计保持在烘箱上方，以增加温度稳定性，并消除通过安装螺钉传递的任何热量。

你可以观看视频，休息后了解更多细节。

【达夫·琼斯】在 [EEVBlog 关于铷频标的一集](http://youtu.be/I55uLRRvLCU?t=6m46s)中很好的概述了不同的晶体振荡器及其特性。

[https://www.youtube.com/embed/B_Y971uY3Nk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/B_Y971uY3Nk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)