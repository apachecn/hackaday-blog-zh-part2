# 用 I2C 接口制作固态继电器

> 原文：<https://hackaday.com/2013/11/01/making-a-solid-state-relay-with-i2c-interface/>

[![](img/75810aa2b7c1dae58668590cb61feea0.png)](http://hackaday.com/wp-content/uploads/2013/10/2013-10-27_triac-bloc.jpg)

由于[Mic]经常收到制作大功率开关板的请求，他最近终于做出了让步，[基于固态继电器设计了上图](http://wemakethings.net/2013/10/27/triac-bloc/)所示的开关板。一些已经接触过市电电源的读者知道，当电压超过零伏时，通常会发生切换。“TRIAC BLOC”能够做到这一点，它还允许测量电源频率。[Mic]然后通过调整其 OSCCAL 寄存器值，使用此 50Hz 调谐至 ATtiny 微控制器的内部振荡器，因此可以在理想的时刻发送切换命令。过零检测通过将电源馈入交流光耦合器来实现。[Mic]发现光耦合器二极管并不相同，因此他必须调整固件以适应时差。

github 上提供了所有资源，我们很想听听您对使用无源器件 R3/C1/L1/R8/C3 实现的电路的详细分析。