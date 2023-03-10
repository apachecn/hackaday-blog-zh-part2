# FindChips 是如何作为 NASA 工程师的黑客起家的

> 原文：<https://hackaday.com/2013/09/09/how-findchips-started-as-a-nasa-engineers-hack/>

几周前，我去 SupplyFrame 拜访了 Hackaday 的新老板。首席执行官[Steve Flagg]问我如何向读者介绍 FindChips。我习惯了人们试图把事情放在我们的头版，所以我为他准备了一个问题:黑客在哪里？令我惊讶的是，他已经准备好迎接我了。"如果我告诉你，这是由美国宇航局的一名工程师发起的黑客攻击，会怎么样？"

事实证明他是对的。他帮我联系了 FindChips.com 公司的创始人兰迪·萨金特。如果你曾经为了让你的生活更简单而拼凑了一个脚本，你会想听听 Randy 是怎么说的。你永远不知道它什么时候会变成一个成熟的初创企业。

### 开始

原来[兰迪]在创建 FindChips 时并不是美国宇航局的工程师，但他现在是了。对于那些不熟悉它的人来说，该网站提供了一个电子元件的统一搜索，它将为你提供来自世界各地供应商的库存和价格明细数据。这种服务在 20 世纪 90 年代根本不存在，[Randy]花费时间访问每一个可能的供应商网站，搜索他设计中的组件，这让他非常沮丧。所以他做了任何优秀黑客都会做的事，他写了一个脚本来帮他做这件事。

### 剧本及其传播方式

他想出的是一个 Perl 脚本，它使用 web 抓取为他做搜索。[Randy]回忆起当时没有可用的解析库(例如:Beautiful Soup ),所以他编写了一切来获取数据，并用正则表达式来理解它。软件是脆弱的，因为一个供应商网站上的小变化可能会破坏刮刀，所以他编写了可以搜索一般地标的库。例如，他们查找任何表，并匹配两个列标题来识别它。这样，如果添加或删除了其他列，或者更改了表的顺序，脚本仍会运行。

![seattle-robotics-society](img/45b04eeeacc30afe3a2d5e02d55d18b7.png)

1998 年的某个时候，第一个版本在他家里的 DSL 连接上运行。他发现这在他自己的工作中是非常宝贵的，因此他在西雅图机器人学会的月度会议上做了报告。30-40 人左右的群体，大部分空闲时间都在做机器人；这对他们来说再好不过了。所以毫不奇怪，流量很快就超过了他的家庭连接。他继续前进，将运行网站的机器移植到[的一个托管设施](http://en.wikipedia.org/wiki/Colocation_centre)。

### 供应商们开始注意到这一点，所以兰迪侵入了他们的搜索算法

关于网络抓取的事情是，如果你开始使用大量的流量，服务器所有者将会注意到。[Randy]回忆起供应商通常以两种不同的方式接近他。一些人要么要求他停止抓取他们的网站，要么直接屏蔽他。但是其他人有相反的反应。他们告诉他，他的网站是他们最大的流量来源。起初这听起来很棒，但是因为他使用了网络搜索界面，它的副作用是降低了实际用户搜索供应商网站的速度。解决方案是建立一个系统，每天将供应商股票数据库的副本上传到 FindChips。

这不是一个 API，而是对他们数据的直接访问，这让 Randy 再次回到编码椅上，重新编写他的脚本来查询服务器端，而不是网络抓取。他告诉我，他修改了 grep 命令来帮助这个搜索过程，并最终从 db 查询中获得了比供应商自己能够提供的更快的返回。看到这一成功，不久更多的供应商也加入进来。

### 我们现在在哪里

![findchips-logo](img/b24f42af8767cad09cf2fc3c9fbd528b.png)[Randy]在 2010 年将网站卖给了 SupplyFrame。当然，它不是一家像苹果那样大的公司。但是故事是沿着同一条线的。他开发它来解决自己的问题，向一个业余爱好组织炫耀，这个组织无疑是今天黑客空间的前身，然后把它变成了一个相当大的网络初创公司。这不仅令人印象深刻，而且鼓舞人心。也许我们搞的项目有一天会对广大观众有用？

如今，除了是美国宇航局艾姆斯研究中心的计算机科学家之外，[Randy Sargent]还是谷歌的访问科学家和卡内基梅隆大学的高级系统科学家。他现在最兴奋的项目之一是超级时间机器。它捕捉并提供数十亿像素规模的延时摄影。

[ [兰迪头像的图片来源](http://www.jhfestival.org/jhsymposium/speakers.htm)