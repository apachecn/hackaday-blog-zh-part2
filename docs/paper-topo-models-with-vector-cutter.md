# 使用矢量切割器的纸张拓扑模型

> 原文：<https://hackaday.com/2015/04/18/paper-topo-models-with-vector-cutter/>

如果有一个科学展即将到来，这将胜过任何 2D 海报。这是 Poľana.一座不活跃的斯洛伐克火山的三维地形图[Peter Vojtek]想出了一个简单的方法来使用 Ruby 生成 SVG 拓扑模式。

地形数据可通过 MapQuest API 获得。您应该能够对世界的任何部分进行建模，但是具有最大高程差的区域将会产生最有趣的结果。这项工作首先使用地图坐标定义一个矩形区域，并决定步骤的数量(代表这个矩形的纸张)。然后将数据分割成每个切片的表格，转换成 SVG 点，并为刀片切割机生成一个文件。当然，你可以升级游戏，用激光从更大的库存上切割下来。如果你有激光切割纸张的技巧，请告诉我们。我们[在尝试这种方法时大多看到了失败](http://hackaday.com/2014/03/27/fail-of-the-week-secret-agent-style-book-hideaway/)。

在[Peter 的]文章中解释的红色模型使用小的交叉片来固定切片。我们喜欢蓝色模型的外观，它在立面图中包含了这些十字。他没有具体解释这一点，但这应该很容易理解——旋转矩形并再次执行切片，对吗？

如果你想从地形中寻找更多的乐趣，我们一直很喜欢[卡罗琳的][测深学书籍](http://hackaday.com/2013/10/03/making-a-bathymetric-book-by-hand-and-searching-for-an-easier-way/)。