# 用于制备啤酒酿造颗粒的制麦窑控制器

> 原文：<https://hackaday.com/2012/10/12/malting-kiln-controller-for-preparing-beer-brewing-grains/>

![](img/77c64c89da67b4e01ba403012a505eb0.png "malting-kiln-controller")

一个快速入门是为了:当谈到爱好酿造有两种主要类型，提取酿造和全谷物酿造。前者使用一种在工厂里从谷物中提取的糖浆，而后者增加了自己动手的步骤。但是在这两种情况下，酿造谷物都已经发芽了。这是一个浸泡谷物，然后在窑中烘干的精细过程。[理查德·奥利弗] [建造了他自己的麦芽窑控制器](http://www.blueleafsoftware.com/Resources/EmbeddedSand/Malt_Kiln)为他的家庭酿酒仪式增加了预备步骤。现在，他唯一没有亲自做的事情就是种植谷物(也许还有培养酵母)。

他最初的设计是用食物脱水机来进行干燥，但是因为温度不合适，所以没有成功。新建筑使用 300 瓦热风枪的陶瓷加热元件。一个鼓风机引导空气通过元件，进入作为窑的木箱。Arduino 监控加热的空气，使其保持在最佳位置。他包括了一个易于监控的图形用户界面，在休息后的视频中显示。

[https://www.youtube.com/embed/zz7VIS3qEPU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/zz7VIS3qEPU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)