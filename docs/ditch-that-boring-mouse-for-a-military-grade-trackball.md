# 抛弃无聊的鼠标，改用军用轨迹球

> 原文：<https://hackaday.com/2013/06/12/ditch-that-boring-mouse-for-a-military-grade-trackball/>

![military-grade-trackball](img/a663738d0f234c674f7358be3ae0d447.png)

这种类型的黑客攻击的坏消息是，现在[托梅克·杜布罗尼克]需要在他的桌子上开一个洞来放置这个东西。他得到了这个通过 USB 接口工作的军用轨迹球。很旧了，可能是钝器。但正如视频所示，它仍然是一个很好的输入设备。

他在[Allegro](http://en.wikipedia.org/wiki/Allegro_(auction_website))——一个类似于易贝的波兰拍卖网站——上找到了这个硬件，只花了 20 美元。[的原始电路](https://hackerspace.pl/~tomek/trackball/top_anno.jpg)没有太多意义，但用旧示波器进行了一点探测，让他建立了与一些 TI 54xx 部件读取的编码器的连接。显然，他们使用与 7400 零件相同的逻辑，但却是军用级别的。他选择了 ATmega32u4 开发板作为替换控制板。该芯片具有原生 USB 支持，因此剩下的只是像 HID 输入设备一样传递数据的问题。他的代码甚至允许他使用这些按钮在光标移动和窗口滚动之间切换。

在华沙黑客空间的朋友们的提示下，[Tomek]将他的帖子翻译成了英文。如果你感兴趣，这是波兰文的原文。

[https://www.youtube.com/embed/7ZbHHgNU2dw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/7ZbHHgNU2dw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[谢谢 Sergiusz]