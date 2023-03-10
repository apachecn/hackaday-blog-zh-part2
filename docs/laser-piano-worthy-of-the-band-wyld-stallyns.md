# 配得上“怀尔德·斯塔林斯”乐队的激光钢琴

> 原文：<https://hackaday.com/2014/07/02/laser-piano-worthy-of-the-band-wyld-stallyns/>

![Laser Piano uses Arduino](img/69b9774d5c933c0732f00928f7a096e5.png)

elecfreaks 的[Robi]和[Kathy]写了一篇关于他们刚刚制造的激光钢琴的文章。代替按键，用户打破激光束来触发声音。

几个激光指示器二极管并联在一起，安装在一个盒子里，在这种情况下是纸板。激光二极管瞄准位于盒子另一侧的光电池。每个光电管都连接到 Arduino 上的数字输入引脚。当 Arduino 从其中一个光电池感应到状态变化时，意味着光束被中断，它会播放存储在外部 JQ6500 声音模块中的适当波形文件。

[Robi]承认有一些需要改进的地方，具体来说就是扳机反应时间和钢琴听起来太单调了。如果你有任何想法，请在评论区留下。

如果你想建造一个，材料清单和 Arduino 代码都列在上面的网站上。我们在过去展示过一些其他有趣的基于激光的乐器，比如这把[吉他](http://hackaday.com/2009/07/13/the-prism-laser-synth-guitar/)，这把[竖琴](http://hackaday.com/2013/10/30/impressive-laser-harp/)和这把[竖琴](http://hackaday.com/2009/12/23/laser-harp/)。

“要互相优秀！”

[https://www.youtube.com/embed/QWdmwE-QR6s?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/QWdmwE-QR6s?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)