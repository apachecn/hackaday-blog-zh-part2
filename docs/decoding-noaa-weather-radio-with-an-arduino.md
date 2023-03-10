# 用 Arduino 解码 NOAA 天气广播

> 原文：<https://hackaday.com/2012/07/27/decoding-noaa-weather-radio-with-an-arduino/>

![](img/d0ef68676181d1efc80cc1b34cdb4e68.png "same-weather-radio-decoder")

美国国家海洋和大气管理局负责广播气象电台使用的信号。他们使用一种称为特定区域消息编码(SAME)的协议，并且[Ray Dees]最近发布了一个 Arduino 库，可以让你解码相同的消息包。

他没有提供调谐无线电信号的方法，但是首先你可以使用他指向的音频样本。实际的广播发生在 162.400 MHz 和 162.550 MHz 之间的七个频率之一上，但是音调也在电视和无线电警报上广播。一旦你有了音频，它就被送入一对 XR-2211 音频解码器。这为 Arduino 提供了三个接口引脚。

在天气警报或警报系统测试开始时吸引你注意力的恼人噪音实际上是相同数据包的声音。从这些音调中，该系统将能够解码所发出的警报类型，以及它所影响的地理位置。如果你有兴趣了解更多关于同一主题的信息，请点击[查看维基百科关于主题](http://en.wikipedia.org/wiki/Specific_Area_Message_Encoding)的文章。