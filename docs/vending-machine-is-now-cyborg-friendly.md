# 自动售货机现在是电子人友好的

> 原文：<https://hackaday.com/2014/03/25/vending-machine-is-now-cyborg-friendly/>

![OZ6dlvn](img/c0a0241c8947ba0c834890157d41b9e8.png)

你不讨厌为了买东西而掏出钱包或手机吗？如果你挥挥手就能通过这种方式转账会怎么样？嗯[大卫]做到了，所以他决定做点什么。他在自己的黑客空间 FamiLAB 制造了一台电子友好型自动售货机。

问题是，从技术上来说，自动售货机不是他可以摆弄的……所以他不得不在不实际修改机器本身的情况下完成这项工作——我们承认，这实际上让它变得更有趣了！

但是首先，为什么[大卫]要这么做？他是机器人还是什么？嗯，不完全是，但他对生物技术相当热情(我们现在是这么称呼它的吗？)——不管怎样，他手里有 [NFC 植入物](http://hackaday.com/2013/10/30/hackaday-interview-with-amal-graafstra-creator-of-xnt-implant-chip/)，指尖有[磁铁](http://gizmodo.com/5895555/i-have-a-magnet-implant-in-my-finger)给他第六种“电觉”。为了最大限度地利用这些增强的能力，他组装了这个聪明的 NFC 信用卡模拟器。

为了读取他的手，他使用了贴在机器前面的 Adafruit RFID/NFC 屏蔽，并使用 Arduino Mega 2560 来控制它。为了摆弄信用卡单元，他在它旁边放了一个螺线管，离得很近，当他的信息通电时，信用卡机器就能读取它。不管你喜不喜欢电子人行动本身，大卫的组合是相当不可思议的。如果你有兴趣了解更多，他在 GitHub 上有详细的说明和材料。

[https://www.youtube.com/embed/jQZdyhS1wVk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/jQZdyhS1wVk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

或者，你可以得到一个 NFC 戒指……或者对于电子感应，[一个钕环磁铁。](http://hackaday.com/2012/01/02/give-yourself-a-sixth-sense-on-the-cheap/)