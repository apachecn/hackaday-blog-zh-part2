# 带有网状网络传感器的低成本模块化高空气球跟踪器

> 原文：<https://hackaday.com/2013/11/21/a-low-cost-modular-high-altitude-balloon-tracker-with-mesh-networked-sensors/>

[![](img/3662e4ef27534467f40534a6cd4dfe29.png)](http://hackaday.com/wp-content/uploads/2013/11/6507343c89ba2e688c63d3b6dae4b77e-media-900x687.jpg)

[Ethan]刚刚告诉我们他和几个同事去年为他们的高级设计项目做的一个项目。这是一个低成本的开放硬件/软件[高空气球跟踪器](http://protofusion.org/wiki/opentrack)，它的传感器与主节点形成网状网络。后者(如上所示)包括一个 ATmega644，一个机载 GPS 模块(NEO-6M)，一个微型 SD 卡插槽，一个 300mW [APRS](http://en.wikipedia.org/wiki/Automatic_Packet_Reporting_System) (144.39MHz)发射机，最后是插头，用于插入 XBee 无线电。因此，该平台负责从从属平台获取无线数据，将其存储在 uSD 卡中，同时通过 APRS 传输气球位置和其他数据。有趣的是，为了保持设计的低成本，他们选择了相对便宜的模拟无线电模块($~40)，并将输出信号的 AFSK 调制与硬件 PWM 输出和正弦波查找表结合在一起。

从节点由“从主板”组成，主板上可以插几个子板:盖革计数器、大气传感器、摄像机控制/加速度计板。如果你想构建自己的系统，请务必查看本页，其中包含所有必要的说明和资源。