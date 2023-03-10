# 向软件定义无线电添加更多频率

> 原文：<https://hackaday.com/2012/07/08/adding-more-frequencies-to-you-software-defined-radio/>

![](img/543cbf3cf6d80d208647fca1ad8b5e56.png "radio")

[regveg]正在寻找一种方法来接收他的电视调谐器软件定义的无线电加密狗可以接收的正常 64-1700MHz 范围之外的信号。在互联网上找到一些 100 美元以上的上变频器后，他[偶然发现了一个 DIY 项目](http://george-smart.co.uk/wiki/FunCube_Upconverter)，该项目大大扩展了他的 RTLSDR 可以接收的频率。

[George]的上变频器使用外差法来增加 SDR 加密狗接收的频率。基本思想是将来自天线的信号与 100MHz 频率振荡器混合。最终输出将为λ + 100MHz 和λ–100 MHz，允许 SDR 电视调谐器适配器接收更宽的频率范围。

现在[regveg]有了一个电路板和原理图，可以用他的电视调谐器适配器接收任何东西。有趣的是，这款上变频器包含不到 10 美元的零件，并且由于单面结构和通孔零件，很容易在家里蚀刻。

顺便说一句，[Andrew]几天前发了一条提示，告诉我们他的 RTL 加密狗[没有任何 ESD 保护](http://ncrmnt.org/wp/2012/06/30/rtl-sdr-static-protection/)。这是一件非常糟糕的事情，但好消息是修复非常便宜:只需[焊接一个 10 美分的二极管](http://octopart.com/bav99-fairchild+semiconductor-13167770)就可以了。