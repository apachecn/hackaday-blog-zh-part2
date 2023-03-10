# 莫尔斯解码器的精益和性感的搜索算法

> 原文：<https://hackaday.com/2014/11/15/morse-decoders-lean-and-sexy-search-algorithm/>

通常我们以莫尔斯电码为中心的项目是为了帮助你练习传递信息。这一个采取了一个策略，建立了一个自动解码器。我们认为[Nicola CIM mino]的项目非常值得一提，因为他解释了麦克风输入信号的数字信号处理。干得好。但他才刚刚开始热身。

真正让它脱颖而出的是[一个出色的算法，它允许使用一个只有 64 字节的查找表将莫尔斯语转换成 ASCII 码](https://github.com/nicolacimmino/MorseDecoder)。这为 A-Z 和 0-9 提供了足够的空间，不会发生冲突，但可以扩展以容纳更多的字符。下面是算法如何工作的简明描述，但请确保您花时间完整阅读[Nicola 的]项目描述。

> 该算法可以描述如下。使查找字符串中的索引为零。具有 64 的初始破折号跳跃大小。在每个接收到的元素(点或破折号)处，将初始破折号跳转减半，然后如果接收到点，则将查找字符串内的索引增加 1，如果接收到破折号，则增加破折号跳转大小。重复，直到到达一个字母分隔符，在这一点上，查找字符串内的索引将指向对应于解码莫尔斯码的 ASCII。

你以前听说过这种技术吗？如果有，请在下面的评论中告诉我们。在你跳过这一步之前，要意识到[魔法莫尔斯使用了一种不同的技术](http://hackaday.com/2014/01/17/magic-morse-arduino-trainer/)。