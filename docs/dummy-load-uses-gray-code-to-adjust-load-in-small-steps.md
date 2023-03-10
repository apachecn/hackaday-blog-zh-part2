# 虚拟负载使用格雷码以小步长调整负载

> 原文：<https://hackaday.com/2012/10/09/dummy-load-uses-gray-code-to-adjust-load-in-small-steps/>

我们对为自己制造这样的虚拟负载并不感兴趣。但是，当您阅读构建描述时，其设计背后的概念是一个很好的精神练习。[Pabr]想要制造一个虚拟负载，用来测试一个廉价制造的气体发生器。他希望它尽可能简单，同时提供一系列不同的负载。他想出的是[这种单调可调的负载测试器，它使用格雷码来切换](http://www.pabr.org/grayload/grayload.en.html)。

休息后的视频很好地解释了设计的动机。格雷编码确保一次只有一位发生变化。他用二进制代码从 7 (0b0111)转换到 8 (0b1000)的例子来说明这一点的重要性。三位数关了，一位数开了。由于他使用灯泡作为负载，这将关闭 700 瓦，然后打开 800 瓦。功率突然增加会导致发电机引擎出现各种问题。但他连接的系统将确保开关的每一次翻转都以更小的步伐移动。

[https://www.youtube.com/embed/5vAJSe8pwMA?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/5vAJSe8pwMA?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)