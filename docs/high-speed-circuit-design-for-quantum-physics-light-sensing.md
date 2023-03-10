# 量子物理光传感的高速电路设计

> 原文：<https://hackaday.com/2013/04/04/high-speed-circuit-design-for-quantum-physics-light-sensing/>

![high-speed-sensor-sampling](img/c82224a0087713211907a44fd08d9c22.png)

[Limpkin]以设计电路为生。这块板是他最近的项目之一，虽然他的技术比我们的经验超前好几光年，但他很好地解释了他是如何组装这块板的。

他的任务是[测量两个光电二极管](http://www.limpkin.fr/index.php?post/2013/03/01/Amplifying-nanosecond-pulses-for-quantum-physics-experiments)的光强。这些元件拾取的预期脉冲持续时间将小于 1 纳秒，这给他带来了一些特殊的设计限制。为了记录这个信号，他在每个输入端使用三个级联运算放大器。为了避免来自射频干扰的错误读数，他还设计了屏蔽，你可以在电路的大部分周围看到。

他为 THS3202 运算放大器选择的封装非常有趣。他没有采用包含散热垫的封装，因为他不想中断电路板下侧的接地层。为了防止部件熔化，他添加了一个接触封装顶部的铝垫片，然后是一个覆盖整个屏蔽框架的散热器。在未来的修订版中，他认为他将转向四层板，这样他们就可以选择 MSOP 的软件包为他工作。