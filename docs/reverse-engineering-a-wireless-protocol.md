# 对无线协议进行逆向工程

> 原文：<https://hackaday.com/2013/07/01/reverse-engineering-a-wireless-protocol/>

![logic](img/15a6081fbe85a4bf1b9551b58f5eea33.png)

像所有优秀的修补匠一样，[安德鲁]决定弄清楚他的无线安全系统是如何工作的。是的，这是[逆向工程](http://cybergibbons.com/category/alarms-2/friedland-response-reverse-engineering/)中的一次练习，也是我们迄今为止看到的最好的一次。

在拿出手持频谱分析仪和电视调谐器 SDR 之后，安德鲁打开了一些设备，看了看电路板。键盘、PIR 传感器和基站都使用 TI 无线电芯片 CC11xx 系列，该芯片使用 SPI 与微控制器通信。

将逻辑分析仪直接连接到无线电芯片上并直接读取比特，[Andrew]开始获得一些非常好的数据，尽管很难理解。根据安全系统规格，他知道它使用的是“20 位代码”，但他从 SPI 总线上读取的数据包是 48 位长。这部分代码可能是系统的地址，但是系统究竟是如何读取它的传感器的呢？

解决这个问题最简单的方法是切换几个传感器，观察传输的数据。凭借良好的推理，[安德鲁]找出了[报警系统的代码是如何工作的](http://cybergibbons.com/uncategorized/reverse-engineering-a-wireless-burglar-alarm-part-6/)。这个理论通过将一个无线电[连接到一个 Arduino](http://cybergibbons.com/uncategorized/reverse-engineering-a-wireless-burglar-alarm-part-7/) 上进行测试，他的怀疑得到了证实。

虽然[Andrew]在逆向工程方面的冒险只对使用这种安全系统模型的人有好处，但这是一个很好的洞察如何拆开事物并理解它们。