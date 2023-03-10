# 可视化 RF 驻波

> 原文：<https://hackaday.com/2015/08/06/visualizing-rf-standing-waves/>

驻波是很多人都有工作知识的话题之一，但似乎很少有人真正掌握。业余无线电爱好者会告诉你他的天线的驻波比(SWR)，他甚至会在房间里放一个测量仪来测量。他会知道 1.1 比 1 的 SWR 是好事，但 2 比 1 就不那么好了。不过，请他解释一下驻波到底是什么，他很可能会举手示意。但是[Allen]，一个也被称为[w2ew]的火腿，刚刚发布了一个优秀的视频，通过[沿着一条开放的传输线](https://www.youtube.com/watch?v=M1PgCOTDjvI)测量信号来解释驻波。

[![[Source: Wikipedia]](img/1b9124e392a6c44f7049f78704283529.png)](https://hackaday.com/wp-content/uploads/2015/08/350px-standing_wave_2.gif) 

【来源:维基百科】

要真正理解驻波，你得记住两件事。首先，当任何种类的波经历传输介质阻抗的变化时，它们将至少部分被反射。典型的例子是射频传输线路末端的开路或短路，它会将输入的射频信号完美地反射回信号源。第二，在同一介质中传播的波相互重叠，它们的波峰和波谷可以相加。如果两个波峰在一起，它们会相互加强；如果波峰和波谷在一条线上，它们会互相抵消。

一切都很好，但是驻波实际上在传输线中*看起来*像什么？[Allen]使用带线进行演示，带线只是传输线的一个开放部分。借助一个特殊的射频探测器探头，[Allen]能够沿着带状线扫描，并显示移除线路终端所产生的 2.4GHz 驻波的几个周期。波节和反波节在带状线上明显分开，分开的距离与波长成正比。

对我个人来说，这真是大开眼界。现在我不仅明白了驻波从何而来，还明白了波节和反波节映射到一条线上的物理位置，这些物理位置是驻波频率的特征。简单的概念，但没有这种可视化，它只是从来没有点击。为了让你大开眼界，一定要看看[Eliot Williams]最近关于输入阻抗的“跟我说”专栏。

[https://www.youtube.com/embed/M1PgCOTDjvI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/M1PgCOTDjvI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)