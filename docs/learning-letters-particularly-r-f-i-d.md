# 学习字母，尤其是 R、F、I 和 D

> 原文：<https://hackaday.com/2013/06/10/learning-letters-particularly-r-f-i-d/>

![8993376562_55ff3846b3](img/7ec72cd58a444c230f30a3f40716ce4d.png)

在(约哈内斯)在旧货市场买了一个玩具——一个 Leap Frog 字母工厂发音器——之后，他认为自己可以做得更好。该玩具最初要求儿童找到一个字母，在从塑料盆中挖出 26 个塑料字符中的一个并将其放在字母工厂的传感器上后，将播放一小段音乐。[【yoha nes】版本做了同样的](http://tinyhack.com/2013/06/09/rfid-based-toy-for-toddler/)，但是因为是他自己做的，所以它的可扩展性更强。

[yohanes]版本的字母[带有 RFID 标签](http://www.aliexpress.com/item/EM-ID-CARD-4100-4102-reaction-ID-card-125KHZ-RFID-Card-fit-for-Access-Control-Time/851364985.html)。这与廉价的 [RFID 模块](http://www.aliexpress.com/item/1-Set-New-125Khz-125-khz-RFID-Mini-Module-kit-Kits-For-DIY-freeshipping/844714959.html)和蓝牙模块相结合，意味着树莓派可以从房间的另一端读取 RFID 卡。从那以后，很简单的事情就是写一些 Python 向他蹒跚学步的孩子要一封信，读取来自蓝牙的比特，并记录分数。

这座建筑远未完工。[yohanes]仍然需要通过添加印度尼西亚语和泰语来使他的构建多语言化。也有可能增加一个拼写游戏，使它更有趣。