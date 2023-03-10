# ZX81 克隆着色机

> 原文：<https://hackaday.com/2015/05/20/colorizer-for-zx81-clone/>

[danjovic]是一个老式电脑爱好者，他的收藏中有几台旧电脑。其中有几个 TK-85 单元——由巴西 Microdigital Eletronica 公司制造的 ZX81 克隆体。TK-85 输出单色视频输出。当[danjovic]获得一台 SyncMaster 510 电脑显示器时，他着手构建一个电路来“着色”ZX81 克隆体的输出。

SyncMaster 510 支持 15kHz RGB 视频刷新率，因此他认为将其连接到 TK-85 应该很容易，TK-85 内部有视频和复合同步信号可用。 因此，如果他能使用电阻将视频信号的幅度降低到 0.7Vpp，并将该信号连接到监视器上的一种原色，例如绿色，那么屏幕上应该有绿色背景的黑色字符。

在他做这些之前，他首先必须调试和修复 TK-85，它似乎有几个与年龄相关的问题。在更换了几个老化的集成电路插座后，他能够让它运行起来。他将电线直接焊接到一个逻辑芯片上，该芯片上有视频和同步信号，以及+5V 和 GND 连接，并将它们连接到试验板上。然后，他测试了由 TTL 多路复用器、DIP 开关和电阻组成的电路。这很有效，但不像预期的那样，经过一番挖掘，他推断这是由于视频信号中缺少后沿。从维基百科来看，“*后沿*是水平同步脉冲结束(上升沿)和活动视频开始之间的每条扫描线的部分。它用于恢复黑电平(300 mV。)模拟视频中的参考。在信号处理方面，它补偿同步脉冲后的下降时间和建立时间。

为了实现后门廊，他参考了他遇到的一个[老黑客](http://translate.googleusercontent.com/translate_c?depth=1&rurl=translate.google.com&sandbox=0&sl=auto&tl=en&u=http://victortrucco.com/TK/ZX81Backporch/ZX81Backporch.asp&usg=ALkJrhhcYL7fBAIMrhBSja8Hr03Jzz2dYA)，涉及解决 ZX81 中的一个类似问题。最终，它可以通过一个 RC 滤波器和一个二极管轻松实现。完成后，他现在能够为前景和背景颜色选择任何 RGB 值。最后，他制作了一个小小的 [PCB 来容纳多路复用器](http://translate.google.com/translate?sl=auto&tl=en&u=http://danjovic.blogspot.com.br/2015/05/placa-do-adaptador-rgb-kolour.html&sandbox=0&usg=ALkJrhjQTvlEZjLyzgirhWGKr0PqeIgMxQ)、双列直插式开关和电平转换电阻。对于那些感兴趣的人来说，他还在一篇由四部分组成的博客文章中记录了他对 TK-85 的[修复。](http://translate.google.com/translate?sl=auto&tl=en&u=http://danjovic.blogspot.com.br/&sandbox=0&usg=ALkJrhjPCMN4SvNzgth_-IpexCce5zdpfA)