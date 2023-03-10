# 点亮通向正确电阻器的路

> 原文：<https://hackaday.com/2014/02/15/light-your-way-to-the-correct-resistor/>

![click-and-see](img/f476a058a8d1471ae2345d6532e03a19.png)

谁没有组件存储的问题(说真的，在评论中告诉我们你的秘密)？如果你能把你的备件整理好，仍然很难弄清楚你到底把它们放在哪里了。给抽屉贴标签是一回事，但如果你有成百上千个抽屉呢(我们正在关注你，每一个已经存在几个月以上的黑客空间)。这个项目通过[点亮从你的计算机化库存中选择的库存的组件抽屉](http://blog.modulowo.pl/click-and-see/) ( [翻译](http://translate.google.com/translate?sl=auto&tl=en&js=n&prev=_t&hl=en&ie=UTF-8&u=http%3A%2F%2Fblog.modulowo.pl%2Fclick-and-see%2F))，为井井有条的零件存储添加了一个数字提示。

这个想法是，你所有的零件都被分配到电脑的一个抽屉空间。当您进入索引并选择零件时，指定的抽屉会被 LED 照亮。这里的设置是一个 I2C LED 驱动器的分线板，它与 Raspberry Pi 接口，但这个概念应该很容易在任何系统上实现。

需要帮助来让你有足够的组织能力来实现它吗？我们也是。也许[重温这个存储综述](http://hackaday.com/2011/07/26/hackaday-links-july-26-2011/)会有所帮助。