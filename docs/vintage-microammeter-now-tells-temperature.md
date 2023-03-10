# 老式微安表现在可以显示温度

> 原文：<https://hackaday.com/2015/05/18/vintage-microammeter-now-tells-temperature/>

[Craig]发来了一个小技巧，他用几个零件将一个旧的模拟微安培计转换成温度计。复古模拟仪表有一定的魅力，旧仪表内部有足够的空间来容纳微小的试验电路板电路和三节 AA 电池，将其转换成一个看起来很酷的中心装饰品，也很有用！

他使用 3 引脚 [MCP9700](http://ww1.microchip.com/downloads/en/DeviceDoc/20001942F.pdf) 模拟温度传感器连接到[LTC 1541](http://cds.linear.com/docs/en/datasheet/15412fd.pdf)——一个集比较器、运算放大器和带隙基准电压于一体的封装。温度计显示每摄氏度 1uA，输出每摄氏度 1mV，用于外部温度监控/数据记录，功耗约为 20uA。虽然构建本身非常简单，但休息之后，[Craig]花时间在视频中回顾了他做出的每个设计决定。首先是他的电路设计，然后是器件及其值的选择。对于想要了解更多基于精密运算放大器的设计的人来说，这个视频是必看的。

随着时间的推移，三节电池会耗尽，像这样的电路需要稳定的基准电压。这由 LTC1541 的带隙基准电压负责。这样就无需使用额外的电压调节器，使电路可以在 4.5V 至 3.3V 的电压下工作。休息后观看视频，听[Craig]介绍其工作原理。我们不确定它对环境温度变化的响应速度有多快，因为传感器被封装在血糖仪内部，所以可能在背面设置一些通风口，或者将传感器拿出来可能是个好主意。

[https://www.youtube.com/embed/PIT7x9hy16w?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/PIT7x9hy16w?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)