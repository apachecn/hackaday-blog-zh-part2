# 20 美元全球定位系统/GLONASS/北斗接收机

> 原文：<https://hackaday.com/2014/01/17/20-gpsglonassbeidou-receiver/>

无论是反向地理缓存还是无人机遥测系统，在一个项目中安装 GPS 模块已经司空见惯。然而，这些 GPS 模块很贵，而且它们只监听 GPS 卫星，而不是俄罗斯的 GLONASS 卫星或中国的北斗卫星。 [NavSpark 有能力监听所有这些定位系统，](http://www.indiegogo.com/projects/navspark-arduino-compatible-with-gps-gnss-receiver)同时是一个价格约 20 美元的 Arduino 兼容板。

NavSpark 内部是一个 32 位微控制器内核(不，不是 ARM。LEON 拥有 1 MB 的闪存和 212kB 的内存，马力强劲。附加在这个核心上的是一个 GPS 单元，它能够监听 GPS、GPS 和 GLONASS，或者 GPS 和北斗信号。

理论上，对于任何需要全球定位和强大微控制器的应用来说，这都是一款令人印象深刻的主板。也可以选择使用两块电路板和有源天线来捕捉载波相位信息，从而将这种设置的精度降低到几厘米。确实很酷。

感谢[Steve]发送此邮件。