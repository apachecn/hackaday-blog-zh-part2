# 采访特斯拉电池黑客[wk057]

> 原文：<https://hackaday.com/2014/11/11/draft-an-intverview-with-tesla-battery-hacker-wk057/>

早在九月份，我们就报道过[wk057]和他的[特斯拉 Model S 电池拆卸](http://hackaday.com/2014/09/13/tesla-model-s-battery-teardown/)。从那以后，我们花了一些时间去找他，问了几个问题。

**你提到你有一辆(非黑客)特斯拉 Model S，你觉得这辆车怎么样？**

这是我开过或拥有过的最好的车。不想太投入，但是，我喜欢。在不到一年的时间里，我已经跑了将近 20，000 英里，我没有真正的抱怨。软件功能请求…但没有投诉。在将近一年的时间里，我在一周内完成了 1700 英里的多次旅行，获得了一次非常棒的体验……在这之后，我再也不会回到汽油汽车上了。这就像回到马车时代。

与铅酸电池相比，废弃的特斯拉锂电池肯定很贵。是什么让你选择了特斯拉？

实际上，如果你考虑到 Model S 电池已经预先设置为高容量电池组，包含这样做的布线，并且模块比任何铅酸电池组的能量和功率密度都高得多，它实际上几乎比可比的铅酸电池组和所有配件都便宜。

我还没有正式称重，但 Model S 电池的模块大约有 80 磅。80 磅 5.3 千瓦时的电池大约是每千瓦时 15 磅，这是令人印象深刻的。相比之下，一个像样的铅酸电池将有 1 千瓦时多一点(低速率放电容量)，重量几乎相同。

此外，特斯拉包比同样容量的铅酸电池更强大。一般来说，铅酸蓄电池组的容量只有在缓慢放电时才能实现，例如 1/20C。超过这一点，你就会为了权力而牺牲能力。85kWh 的 1/20C 只有 4.25kW，勉强够一个中央空调和一些灯使用而不损失容量。

现在，特斯拉电池组可以在高达 3.75C 的温度下短期放电(基于它在车辆中的放电方式)，并在 1/2C 的温度下持续放电，而不会真正影响电池组的总容量。这意味着我可以运行比铅酸多 10 倍的功率，而总体充电容量没有损失。带来更加灵活的电池解决方案，因为实际上，负载总是很低，甚至不会与 Tesla pack 一起使用，但几乎总是与铅酸有关。

特斯拉电池的充电也更好一些。以 1/2C 的电流给铅酸电池充电，它会沸腾。在 1/2C (42kW)下给特斯拉包充电，它可能会预热几度。哦，高倍率下的充电损耗也比铅酸小得多。总的来说，不用继续谈论技术方面，它只是一个更好的电池，占用更少的空间，更轻的重量，有更多的可用功率。

对于其他的解决方案，可能有很好的理由，但除此之外，这个方案胜出了，因为它肯定更有趣。

点击休息时间阅读我们对[wk057]的采访！

![tesla-4](img/3ff78b99d9a4258ec489368e5d7edbc5.png)

找到一块废旧电池很难吗？花了多少钱？

实际上，当我在考虑我的项目的选择时，我偶然发现了一个列表，上面有一个人在卖一个从 TMC 上捡来的东西。
价格相当昂贵，大约 2 万美元。然而，总的来说，每千瓦时的成本明显低于其他可比选项，尤其是在考虑了我上面提到的因素之后。所以，这是显而易见的。

**买裸 18650 细胞，从零开始建立一个系统怎么样？**

我考虑过这一点，实际上购买了一些，并组装了一个小模块的细胞。许多小时，相当酸痛的手，一个小烙铁烧伤后，我有一个 0.5 千瓦时的包，总的来说，不算时间，每千瓦时的成本是我买的特斯拉包的 2.5 倍。再加上劳动力，价格可能会高出 5 倍以上。肯定不值得。

告诉我们一些关于你的太阳能装置的其他情况。它有多少面板，哪些逆变器？

我用价值不到 30 千瓦(DC)的大型商用太阳能 20%效率 435 瓦电池板(69 块)安装了这个系统，我能以惊人的价格买到它(每瓦 0.8 美元)。

对于逆变器，我现在已经有几个 Outback Radian 系列 GS8048A，8kW 离网型。它们是可编程的，并与我重新配置的特斯拉模块(标称 44.4V，约 1900Ah)完美配合。它们是可堆叠的，所以我计划增加更多，以基本上获得与我从电网获得的相同安培数的交流服务。

有了充电电池，没有太阳能输入，我希望能够运行家庭，不算 Model S 充电，几天没有问题。通过太阳能输入，包括 Model S 充电，它应该可以无限期地作为电力的缓冲。我计划每年发电约 35，000 千瓦时，并以标准的特斯拉风格“不妥协”运行家庭。

![Tesla Model S](img/e137640ff71d4e9faeab2753c91c06cc.png)

你是打算完全脱离电网，还是打算在你的电池组充满电后再卖回电网？

看你怎么看了。我计划完全用我的太阳能装置/电池组为一切供电，从电网中提取零。然而，我没有削减我的网格服务。我选择的逆变器是电网互动的。如果由于某种原因，我需要的电力超过了电池和太阳能所能提供的，他们可以从电网给电池充电。
因此，99.9%的时间我会完全脱离电网，因为我会相应地调整我的设置。电网基本上将是我的备用发电机(连同我实际的备用发电机)。

我根本不打算回售给电网。我最初决定脱离电网，因为在我看来，净计量的概念是有缺陷的。电网不是电池，但这正是许多人用它来计量电网的原因。最终，政策将会改变以反映这一点，而这样做的成本效益可能会很快丧失。脱离电网确保了我能够持续控制我的电力生产和使用。每千瓦时的价格明年可能会跃升至 5 美元(不太可能)，这不会影响我。

如果我产生多余的电力，这可能会在夏天发生，我计划在适当的地方设置几个分流装置来倾倒电力。第一个是我的 Model S，如果有的话，充电不足 90%。接下来是一些气候调整(使温度降低 1 度或升高 1 度，以在房子里“储存”能量)。自动修改当天的池泵计时器计划。把热水再加热几度，等等。不打算把多余的浪费掉，而是以其他形式“储存”起来。将需要一点定制硬件来实现这一点，但这是另一天的项目。:)

你和特斯拉的员工谈论过你的项目吗？他们说了什么？

我和特斯拉的几个人谈过这个项目。他们的标准回答似乎是，他们不能以任何方式支持我的努力，也不会提供关于电池组中任何组件的信息来帮助我。我觉得这很不幸。

拆除包装最困难的部分是什么？

很少有事情能排在一起…
首先，安全。因为我不确定任何线路和组件的确切配置和布局，也找不到任何有关这方面的确切信息，所以在基本上看不见的情况下安全拆卸它所需的额外时间和精力可能是最困难的部分，但肯定是重要的，也是值得的。在这里走错一步可能意味着立即死亡。
其次，背包几乎到处都是用强力胶粘在一起的。这实际上使得拆除变得困难。
第三，搬东西。它很重，将近一吨重。即使我给它装上轮子，也要 4 个人才能把它搬动起来。

![tesla-batt](img/a6a63c7ff4310dfc4fa575319248be9a.png)

有一次，你在背包上安装了脚轮，你有没有考虑过在上面安装一个马达？它几乎看起来像一个卡丁车。

脚轮几乎不能承受包装的重量，当我拆除框架时，有几个已经弯曲了。实际上，我哥哥曾提到过卡丁车的事情，我承认……这个想法曾闪过我的脑海，并会把这个项目引向一个完全不同的方向。一辆有数百英里里程的卡丁车…嗯…

10。你认为你可以给你的特斯拉 Model S 增加电池来增加里程吗？

有趣的是你提到了这个。直接，不。我不认为有任何方法可以通过增加额外的电池来直接增加范围。除了重量方面的考虑，背包需要与现有的背包平行放置才能工作。所以，假设我能以某种方式把这个东西装在车上或车里，这几乎肯定会把车里的电子设备搞糊涂，很可能会以糟糕的结局收场。

然而，我打算间接地尝试一下。我将不得不尽快把我的测试装置(目前我有几个逆变器、电池组和几个太阳能电池板装置)移到它的永久位置。如果我有时间，我可能会在 Model S 的后面连接一半的电池组和一个逆变器。然后我会开车，在路上的某个地方停下来，从后备箱的包里给 Model S 充电。可能毫无意义，但是，肯定是一个有趣的“是的，我做了那个”项目。

**11。你认为埃隆·马斯克会对你用特斯拉电池组挑战太阳能的极限感到高兴吗？**

如果我理解正确的话，我相信埃隆·马斯克已经参与了类似的更多官方项目。至于他是否会对我的打捞包项目感到“高兴”，我说不上来。无论如何，我想他至少会欣赏它的回收利用方面。

**12。如果你可以问埃隆·马斯克任何问题——是关于特斯拉、太阳城还是 SpaceX，你会问什么？**

事实上，我很好奇他对我的特定项目有什么想法，他是否预见到了这样的项目，以及他认为类似的项目现在或将来会对特斯拉产生什么影响。

我们要感谢[wk057]花时间回答我们的问题，并祝他的特斯拉超级家用太阳能系统好运！

![tesla6](img/6d7fa483245f9fec269aa8afc07720b6.png)