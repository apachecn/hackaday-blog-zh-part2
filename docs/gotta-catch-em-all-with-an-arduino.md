# 必须抓住他们，用 Arduino

> 原文：<https://hackaday.com/2014/01/01/gotta-catch-em-all-with-an-arduino/>

![PKMN](img/bee87b5ac104e744ba081ba93327927e.png)

对于你在成为世界上最伟大的训练者的冒险中遇到的每一个口袋妖怪，你都有大约 8000 分之一的机会让那个口袋妖怪变得“闪亮”,或者与正常颜色不同。将一个不寻常的事件放在任何视频游戏中，当然会有一些人将这一功能发挥到实用的极限:[dekuNukem] [c](https://www.youtube.com/watch?v=jyJPsZc-QTM) [创造了 Poke-O-Matic](https://www.youtube.com/watch?v=jyJPsZc-QTM) [，](https://www.youtube.com/watch?v=jyJPsZc-QTM)一种由微控制器驱动的设备，可以繁殖和捕捉闪闪发光的口袋妖怪。

我们以前见过[dekuNukem]自动捕捉闪亮口袋妖怪的[设置，但之前的版本极其有限。它只适用于鱼竿，所以除非你想要一吨闪亮的鲤鱼王，否则早期的设置不是非常有用。](http://hackaday.com/2013/11/05/finding-shiny-pokemon-automatically/)

这个版本使用了两个微控制器——一个 Arduino Micro 和一个 Teensy 3.0——大大扩展了以前的版本。现在，[dekuNukem]的项目不仅可以捕鱼，还可以自动孵化鸡蛋，在草丛中搜索闪闪发光的口袋妖怪，还可以自动命名这些新的闪闪发光的口袋妖怪，并将其存放在游戏内的口袋妖怪存储系统中。

新的和改进的版本工作起来很像老式的钓鱼专用自动口袋妖怪探测器；焊接在按钮触点上的几根电线控制着游戏。Teensy 3.0 使用 SD 卡和 RTC 处理所有捕获的口袋妖怪的数据记录。

[dekuNukem]的所有努力最终得到了什么？一大堆闪亮的口袋妖怪。足够建立一个完全由闪亮之星组成的伟大团队了。

下面的视频，所有代码都可以通过描述中的链接获得。

[https://www.youtube.com/embed/jyJPsZc-QTM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/jyJPsZc-QTM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)