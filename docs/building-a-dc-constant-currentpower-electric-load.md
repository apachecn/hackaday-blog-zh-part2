# 建立 DC 恒流/功率电负载

> 原文：<https://hackaday.com/2013/10/28/building-a-dc-constant-currentpower-electric-load/>

[![](img/34e67280d81184242e70357cbd4c46cb.png)](http://hackaday.com/wp-content/uploads/2013/10/electronicload.jpg)

只看上面的图片，我们很确定大多数黑客读者现在已经猜到这个[电力负载](http://www.kerrywong.com/2013/10/24/building-a-constant-currentconstant-power-electronic-load/)会消耗多少电力。对于那些不知道的人来说，电力负载(或虚拟负载)是一种用于模拟系统负载以进行测试的设备。这在测量电池容量或测试电源时非常方便。

[Kerry]设计的设备的核心是基于 6 个功率 MOSFETs、几个运算放大器和一个 Arduino 兼容的 ATmega328p 微控制器。检测电阻用于测量流过 MOSFETs(以及负载)的电流量，microchip 的 MCP4921 数模转换器(DAC)用于设置电流命令，负载电压由 ATmega ADC 测量。测量后者允许恒定功率负载模式(功率=电流*电压)。在他的文章中，[Kerry]展示了他可以模拟高达 200W 的负载。

[https://www.youtube.com/embed/qSjslZFiRmo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/qSjslZFiRmo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)