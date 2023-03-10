# 用标准模板库给出 Arduino 队列、向量和流

> 原文：<https://hackaday.com/2012/10/22/giving-the-arduino-deques-vectors-and-streams-with-the-standard-template-library/>

![](img/43997e09bae19560747b10c6c8f7d41c.png "duino")

Arduino IDE 与 C++极其相似，但是从你在互联网上找到的草图来看，你永远不会知道它。更简单的 Arduino 项目只需切换 IO 引脚、读取值和在两点之间发送串行数据即可。更复杂的构建属于真正的软件开发范畴，而这正是标准 Arduino IDE 所不具备的。

[Andy]认为更复杂的软件缺乏合适的库是一种可怕的情况[，并决定对此做些什么](http://andybrown.me.uk/wk/2011/01/15/the-standard-template-library-stl-for-avr-with-c-streams/)。他移植了 [SGI 标准模板库](http://www.sgi.com/tech/stl/)，将所有这些有趣的算法和数据结构带到任何 AVR 芯片上，包括 Arduino。

浏览一下[Andy]的 port 中包含的内容，读起来就像是面向对象编程课程的大纲。栈、队列和列表都被切割，字符串和向量也是如此。还包括了和标题中的所有内容，以及一些面向 Arduino 的附加内容，如硬件串行和液晶流。

随着所有这些对象四处浮动，[Andy]说这将对 AVR 中的闪存和 SRAM 的使用产生影响。尽管如此，随着更快更大的 ARM 微控制器的喧嚣，很高兴看到经典的 8 位微控制器变得更加精致。