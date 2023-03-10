# 摩天大楼俄罗斯方块让城市知道你有多好或多坏

> 原文：<https://hackaday.com/2015/01/01/skyscraper-tetris-lets-the-city-know-how-good-or-bad-you-are/>

如果你已经玩了一个多小时的俄罗斯方块，也许是时候在伦敦壳牌中心这个摩天大楼大小的显示器上向世界展示你的技能了。[Benjamin]、[Tom]和他们的“志愿者大军”来到 Shell building，用 182 个联网的无线灯泡、[一些描图纸和聚脂薄膜组装了他们的超级屏幕](https://www.section9.co.uk/posts/2014-12-30-Tetris.html "assembled their super-screen")，从下面的 Jubilee Gardens 创建了一个可玩的界面。

[Benjamin]在他的帖子中没有提供很多技术细节，但是他给了我们一个概述。他通过隔开 14 个 [TP-Link WR702n 路由器](http://wiki.openwrt.org/toh/tp-link/tl-wr703n "TP-Link WR702n routers")实现了所有楼层的完全无线覆盖，每个路由器都运行相同版本的 OpenWRT。这个接口不是[本杰明]的首选，因为他更喜欢接入大楼现有的无线网络；不幸的是，他没有得到大楼网络团队的支持。装有大量由中央桥控制的无线灯泡，由 Python 改编的俄罗斯方块(Benjamin's)每秒钟可以刷新建筑大约 1 到 2 帧。根据他对灯泡接口的描述，我们怀疑他正在使用大家都太熟悉的[飞利浦 Hue 智能灯泡](http://hackaday.com/2012/11/21/giving-siri-control-of-some-smart-bulbs/ "Philips Hue Smart Lightbulbs")来照亮大楼。

如果你没有听说过[法拉第的圣诞讲座](http://www.bbc.co.uk/programmes/p02ftv0l "Faraday's Christmas Lectures")，它们是英国全国广播的“科学特别节目”，在年底播出，由[迈克尔·法拉第](http://en.wikipedia.org/wiki/Michael_Faraday "Michael Faraday")本人于 1825 年创办。这些讲座的目的是向年轻人介绍科学的某些方面。我们以前看过《T4》中的巨型俄罗斯方块，但不是以一种激发如此年轻观众的方式。我们很高兴地看到，软件(Python、LAN 网络)和硬件(ZigBee、OpenWRT)方面的黑客技术入选了今年的特辑。毕竟，为什么麻省理工学院要把所有的乐趣都留给自己呢？

如果建筑规模对你来说太大了，为什么不试试你的示波器呢？

[https://www.youtube.com/embed/NK65ehLFA-U?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/NK65ehLFA-U?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)