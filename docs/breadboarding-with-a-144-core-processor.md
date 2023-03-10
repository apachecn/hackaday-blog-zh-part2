# 搭载 144 核处理器的试验板

> 原文：<https://hackaday.com/2012/10/03/breadboarding-with-a-144-core-processor/>

![](img/aa8dd743fd4b1db0840a18a5936d4c72.png "greenarrays-144-core-processor-breadboarding")

绿色印刷电路板的中心是一个非常小的处理器，有太多的内核。这是[ga 144，由【Andrew Back】在试验板上](http://www.designspark.com/content/hands-144-core-processor)进行试驾。上个月我们看到了多核 Kickstarter 项目[。这将大大降低成本，并让您获得两倍以上的内核数量。但是正如在那个帖子的评论中提到的，缺点是编程语言。该芯片的集成开发环境采用 Forth。](http://hackaday.com/2012/09/28/massively-parallel-64-core-computer-costs-99/)

有一个开发板可用，但[安德鲁]去，而不是一个 QFN 到通孔适配器板，他手工焊接。一旦他可以访问引脚，就可以用与 1.8V 逻辑电平兼容的 FTDI 适配器对芯片进行编程。提供的 IDE (arrayForth)是一个 Windows 专用程序，但它可以在 Wine 下运行。我们跟踪这个项目，看他摆弄 I/O 引脚。但是我们仍然很难想到它的应用。在一个复杂而廉价的 FPGA 芯片世界里，你会用这种处理器做什么？