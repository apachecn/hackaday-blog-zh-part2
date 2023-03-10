# 本周失败:KiCad 中未连接的网络

> 原文：<https://hackaday.com/2014/03/13/fail-of-the-week-unconnected-nets-in-kicad/>

![fotw-unconnected-net](img/5a22a695bfec28e239f29ffec0aa41e6.png)

从上面的标题和图片中，你肯定已经了解了这个星期的失败。我们都经历过。设计一个电路板，把它送到 fab 或者自己蚀刻，然后发现你错过了一个连接。软件中的自动检查应该可以防止这种情况，但是在做小的改动时，很容易忽略再次运行检查。这正是[克林特]在这块板上所做的；[在原理图中留下一个未连接的网络](http://www.cascologix.com/1/post/2013/12/eeeek-something-wicked-this-way-comes.html)，它穿过电路板布局并进入 OSHPark 电路板。

好吧，所以用跳线固定它，这显然是他做的(上图左下方的白线)。但由于这是他的 PCB 的第 3 版，所以发生这种情况很令人不安。失败的主要原因是导致失败的软件功能缺失。KiCad 在电路板布局中没有引脚交换工具。真的吗？我们经常使用 KiCad，并没有意识到该功能的缺失。为了简化电路板布局，[Clint]回到原理图，手动更换一些电阻网络引脚。他通过网表将改变推进电路板布局，没有意识到他留下了一个未连接的输入门。

一点搜索证明，pin 交换可能很快就会来到 KiCad。CERN 的路线图上有他们计划添加到开源 PCB 布局软件中的特性。我们记得很久以前听说过欧洲核子研究中心的计划，并认为我们有特色，但我们能找到的唯一参考是 12 月份[【克里斯·甘梅尔】对一篇帖子](http://hackaday.com/2013/11/10/kicad-video-series-from-concept-to-manufacture/comment-page-1/#comment-1098015)的评论。值得看看他们的计划，这些都是使 KiCad 成为巨头的特征。

我们很快就会没有这个系列的故事线索了。如果你喜欢每周阅读关于失败的文章，请写下你自己的失败，并将链接发给我们。当然，您在互联网上发现的任何失败记录也应该发送给我们。谢谢！

* * *

**[![2013-09-05-Hackaday-Fail-tips-tile](img/4ddcb45ba24697ecb36e5a2da073e8dc.png)](mailto:tips@hackaday.com?Subject=[Fail of the Week]) 每周失败是一个每周三运行的黑客专栏。通过写下你过去的失败和[给我们发送一个故事的链接](mailto:tips@hackaday.com?Subject=[Fail of the Week])，或者发送你在互联网旅行中发现的失败报道的链接，来帮助保持乐趣。**