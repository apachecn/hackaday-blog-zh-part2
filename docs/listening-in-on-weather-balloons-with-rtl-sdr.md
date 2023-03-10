# 用 RTL 特别提款权收听气象气球

> 原文：<https://hackaday.com/2013/01/12/listening-in-on-weather-balloons-with-rtl-sdr/>

![sonde](img/c4e79e666dd7b9099095636ec27b81f2.png)

每天，一天两次，超过 800 个气象气球在世界各地同时发射。这些无线电探空仪传输的数据由政府机构接收，并与气候学家和气象学家共享，以开发气候模型和预测天气。在[卡尔]的家乡奥克兰附近，一个气象气球每天发射两次，由于它们以 403 MHz 传输，他决定使用 USB 电视调谐器直接从大气探测器接收数据。

这个项目的硬件部分包括建造一个为 162 MHz 设计的高增益天线。尽管无线电探空仪以 403 MHz 的频率发射信号，但[Carl]很容易通过他的带外天线接收信号。

对于软件，[卡尔]使用了 [SDRSharp](http://sdrsharp.com/) 和 [SondeMonitor](http://www.coaa.co.uk/sondemonitor.htm) ，允许他将气象气球的编码传输转换成压力、温度、湿度和 GPS 数据。