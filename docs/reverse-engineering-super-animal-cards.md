# 逆向工程超级动物卡

> 原文：<https://hackaday.com/2014/12/11/reverse-engineering-super-animal-cards/>

如果你没有侄女或侄子，我们鼓励你去找一个，因为他们是拆开孩子玩具的绝佳借口。

[Sam]刚买了一些动物主题的交易卡。这些特殊的卡片配有读卡器，当刷卡时，读卡器使用条形码播放每种动物特有的音频。所以[山姆]说服她的侄女，他们应该[画他们自己的条形码](http://incompleteattentionspan.blogspot.com.au/2014/12/super-reverse-engineering-animal-cards.html)。当然，这并不容易:条形码最后会加上奇偶校验位来验证有效读数。但是经过一些可靠的推理和反复试验之后，[Sam]说服了她的侄女，这个世界是靠科学而不是魔法运行的。

但不能就此结束；[山姆]想听所有的动物。打印一堆卡片很繁琐，所以[Sam] [打开读卡器和程序，Arduino 按下按钮，闪烁 IR LED](http://incompleteattentionspan.blogspot.com.au/2014/12/the-revenge-of-super-animal-cards.html) 来模拟刷卡。(Kudos！)现在，她可以轻松地检查动物卡片的所有 1023 个可能值，并播放所有的音轨，她的侄女可以听到比任何孩子都想听到的更多的动物声音。

一路上，[Sam]发现了一些有趣的非动物声音，她认为这些声音是复活节彩蛋，但我们敢打赌，这些声音将来会用在竞赛或宣传图画或类似的东西上。不管怎样，听到比你应该听到的更多的东西是很有趣的。教育下一代小黑客的更好方法是花些时间用纸和笔一起伪造条形码？