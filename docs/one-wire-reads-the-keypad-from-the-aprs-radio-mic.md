# 一根电线读取 APRS 电台麦克风的键盘

> 原文：<https://hackaday.com/2012/05/09/one-wire-reads-the-keypad-from-the-aprs-radio-mic/>

![](img/a10c61bc13ca7865f3e29527f0413f1e.png "aprs-keypad-scanning")

[Shane Burrell]决定花些时间了解一下他的 Kenwood TM-710A APRS 无线话筒的键盘是如何工作的。它使用了一种不同于你想象的技术。通常情况下，按钮网格被扫描成矩阵来检测按键，但这个硬件实际上是对串行线上的脉冲进行计数，以获取每个读数。

股票无线电发送一个稳定的数字脉冲到手机，每个脉冲麦克风拉低线。然后，它使用 4017 十进制计数器来查看返回的内容。如果边沿计数匹配，则意味着没有按下任何东西，但是返回到基本单元的脉冲数量的变化可以用来推断哪个按钮被按下了。

[Shane]继续实施这种控制技术，使用 AVR 芯片代替无线电基站单元。他使用示波器测量脉冲行为获得的数据来编写项目的固件。休息之后，他拍摄了一小段演示，展示了他的发现。

我们不太确定这将如何转化为您自己的自制项目，但用 uC 的两个引脚扫描键盘的想法是非常可取的。当然有[555 定时器频率技术](http://hackaday.com/2011/03/03/keypad-input-scanning-by-a-555-timer/)，但我们总是有新的想法。

[https://www.youtube.com/embed/gAOK225UKWk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/gAOK225UKWk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)