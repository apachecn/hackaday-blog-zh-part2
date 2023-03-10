# 调频的基础

> 原文：<https://hackaday.com/2014/06/26/the-basics-of-frequency-modulation/>

![fm-modulation](img/6509c5d7e03713fb324200f1907e17e0.png)

[brmarcum]通过他的[频率调制和解调](http://www.instructables.com/id/FM-Modulationde-modulation-Circuit/)教程将我们带回到模拟构建模块基础。[调频](http://en.wikipedia.org/wiki/Frequency_modulation) (FM)乍听起来很简单，但理解调频信号调制和解调背后的电子设备可能会令人困惑。我们之前已经[讨论过基本的](http://hackaday.com/2013/09/24/retrotechtacular-fundamentals-of-am-and-fm-radio-communication/)，但是 FM 与广播电台联系如此紧密，以至于搜索经常与 RF、立体声、天线和发射机的参考混淆。

[brmarcum]希望用一种简单的电路来填补这一空白，该电路将音频信号调制为 FM，然后解调并放大它，以便在小型扬声器上播放。他在实验中使用了 Digilent Analog Discovery 工具包，但示波器(一个老式的模拟示波器在这里将是完美的)将用于输出。低端的 555 电路和高端的计算机声卡可以轻松处理信号生成任务。

[brmarcum]显然花了一些时间在他的教程上，但这不是一本关于 FM 调制的大部头书。他将调制和解调电路分解为基本的运算放大器级，并举例说明了每一级后信号在示波器上的表现。这就是这里的美妙之处。通过构建和测试每个部分，任何初次接触模拟的人都可以了解其工作原理。在一些地方，正在发生的事情背后的理论对于指导者来说太深入了，[brmarcum]给出了维基百科的链接。