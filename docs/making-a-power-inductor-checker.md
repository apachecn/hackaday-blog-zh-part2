# 制作功率电感检测器

> 原文：<https://hackaday.com/2013/10/28/making-a-power-inductor-checker/>

![inductor-checker-for-oscilloscope](img/1347e2b553f3d8d77cf46c01b0fd85de.png)

回到基础:无源电子元件有三种:电感、电容、电阻。电感器很容易制造，并且有多种磁芯和线轴套件可供选择。然而，描述一个你刚刚制作的假设线圈是相当棘手的，因为它的电感将取决于测量频率和 DC 偏置电流。这也是【ChaN】[设计上图](http://elm-chan.org/works/lchk/report.html)所示电路的原因。

正如你可能猜到的，RF 爱好者更感兴趣的是电感与频率的关系曲线，而电源电路设计人员更喜欢电感与负载电流的关系(对于给定频率)。上图所示电路的基本原理是在短时间内重复加载一个电感，并用连接到检测电阻的示波器观察电流曲线。当给电感加载时，电流曲线将由两个连续的斜率组成，因为在给定时刻，线圈的磁芯将饱和。通过测量斜率，我们可以计算相应的电感。

[Via [危险原型](http://dangerousprototypes.com/2013/10/23/power-inductor-checker/)