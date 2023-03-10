# 移位寄存器供电的真实蜡烛闪烁

> 原文：<https://hackaday.com/2015/08/29/shift-register-powered-realistic-candle-flicker/>

[Kevin Darrah]最近去一家餐馆吃饭，这家餐馆用了一些便宜的 LED 蜡烛(恶心)，而不是真的。在真正的黑客精神中，他开始注意到编程到假火焰中的模式一遍又一遍地重复。像任何黑客一样，他开始想出一个更好的方法。

现在，我们这些懒惰的黑客可能会抓起一个微控制器，复制并粘贴一些你在互联网上找到的伪随机数生成代码，但不是[Kevin]。他的黑客技术的基础是使用两个连接在一起的移位寄存器，它们被馈送一个时钟信号，还有一个锁存信号，它是由 RC-time 电路产生的同一信号的稍微延迟的版本。

输出的随机性是通过将移位寄存器的输出反馈到异或门而产生的。如果你想了解更多，这种技术叫做“[线性反馈移位寄存器](https://en.wikipedia.org/wiki/Linear_feedback_shift_register)”。它通常被用作穷人的随机数生成器，尽管从技术上来说它不是真正的随机*，从统计上来说它做得非常好。你可以在[Kevin]描述赛道的视频中看到结果。他用电池和太阳能充电电路来完成这个项目。*

 *[https://www.youtube.com/embed/jp9r6_uslyk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/jp9r6_uslyk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)*