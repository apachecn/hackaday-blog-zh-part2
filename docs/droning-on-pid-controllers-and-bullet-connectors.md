# 嗡嗡作响:PID 控制器和子弹连接器

> 原文：<https://hackaday.com/2014/07/07/droning-on-pid-controllers-and-bullet-connectors/>

不是所有的无人机都是多旋翼的——在我们的标题照片中摆姿势的是[梅纳德·希尔](https://www.modelaircraft.org/mag/mhill/hillindex.htm)和赛勒斯·阿多拉希。梅纳德的飞机， [TAM5 又名“巴茨农场的精神”](http://en.wikipedia.org/wiki/The_Spirit_of_Butts'_Farm)，是最小的飞越大西洋的飞机。沿着阿尔科克和布朗从纽芬兰到爱尔兰的路线，这位 6 磅(干重)的模特用了不到 39 个小时完成了旅程。所有这些都发生在 2003 年，是希尔一生成就的顶峰。如果联邦航空局的限制生效，这些类型的追求将在美国被禁止。

#### 飞行控制员

相当多的人认为 Naze32 没有出现在上一期的飞行控制器综述中。我听得很清楚！我将把 Naze 添加到控制器中，这些控制器将在 Hackaday 测试台上进行测试。难的是找到该死的东西！我现在有一架 Acro Naze32 正在去总部的路上。如果我能找到一个完整的版本，我会补充说。

#### **PID 控制器深潜**

我有几个关于比例积分微分(PID)控制器的问题，所以有必要深入解释一下什么是 PID 控制器。PID 控制器通常用于管理温度、湿度或产品流量等参数的过程控制。该算法最初是在 19 世纪晚期设计的，作为控制大型海军船只舵的一种方法。在固定翼无人机中，PID 使飞机的机翼保持水平并保持在航线上。在多直升机中，PID 回路控制航向，但它们也提供稳定的飞行，使四轴飞行器首先能够飞行。对 PID 循环的完整解释超出了一篇文章的范围，但是让我们尝试一个 10，000 英尺的解释。

这是“当前”参数。p 对飞机的性能影响最大。如果风把你的四轴飞行器从水平飞行吹向 30 度的右倾斜，P 这个术语将立即采取行动使四轴飞行器水平飞行。如果 P 值太高，四轴飞行器将越过水平飞行，并开始以另一种方式倾斜。事实上，过高的 P 值会导致四轴飞行器在振荡或“寻找”水平时抖动。P 值太低？四轴飞行器的反应将会非常慢，而且可能永远也不会再次达到水平飞行。

I:这是“过去”参数。I 项抑制了 P 项的过冲和振荡，避免了 P 在设定点上下波动的趋势。就像 P 一样，太高的 I 项会导致振荡。

d:这是“未来”参数，对飞机的行为影响最小。事实上，一些飞行控制员完全不考虑它。如果 P 和 I 过快地接近设定点，则可能会出现超调。在超调发生之前减慢速度。

那么，为什么多翼飞机飞行员害怕 PID 调节呢？很简单，这是一个繁琐的过程。将一名新飞行员和一架未经验证的 PID 值未经调整的飞机结合在一起，你就有了一个令人沮丧的配方——以及坏掉的螺旋桨。当你考虑到至少有 3 组 PID 变量需要调整——俯仰、滚转和偏航时，事情变得更加复杂。一些飞行控制器现在支持多个 PID 值，这取决于飞行的风格。想让你的飞机或多翼飞机像热棒一样飞来飞去吗？你需要一套完全不同的 PID 值，而不是一个温顺的教练工艺。Rolf Bakke (KapteinKUK 本人)[制作了一个视频](https://www.youtube.com/watch?v=YNzqTGEl2xQ)，展示了多机在调整 PID 值时的表现。你可以很容易地看到，只需几个值的调整，quad 就可以从“喝醉”变成“愤怒的蜜蜂”。所有这些都与 Hackaday Testbed 一起出现，它将帮助我发布一些我自己的 PID 调节视频。

#### **黑客日测试平台更新**

至于试验台本身，它几乎完成了！你可以在我的 Hackaday 项目页面上关注进度。组装的大部分相对简单。尽管当然总会有一些障碍。在订购零件进行组装时，我似乎总是会忘记一些事情。在这种情况下，它是 2.5 毫米香蕉插头和电机安装螺钉。

滚轧马达用 3 毫米螺丝固定在框架上。问题是，除非你手头有马达、安装板和无人机框架，否则真的没有办法知道螺丝应该有多长。我有一堆不同长度的 3 毫米螺丝，谢天谢地，有足够的正确长度的螺丝来安装马达。墨菲总是在我身边，因为我不小心抓住了一个 1 毫米长的螺丝，你猜对了，正好拧进了电机的绕组。多。谢天谢地，我有备用的。

![bullet-solder](img/4224f39702027db99a3dd6c2136c07a4.png)子弹型连接器焊接起来很麻烦。有一些夹具有所帮助，但我总是发现自己回到旧的“援助之手”鳄鱼夹。子弹倾向于使用比我们习惯的普通电子产品更细的电线。遥控飞机上使用 14、12 甚至 8 号电线。带有表面贴装头的低功率烙铁是无法胜任的。这些烙铁没有足够的热量使连接器达到焊接温度。在这里，一个 40 瓦或更好的电源(是的，就是那种可以插在墙上的电源)可能是天赐之物。我用的是一个金属熨斗，有一个宽平的尖端。

![bullet-solder-2](img/bb12c817c44179cd0726cc3d8a5f04fc.png)裸露的子弹头连接器和鳄鱼夹也会产生问题——金属夹会产生更多热量。几年前，一个老前辈告诉我一个技巧来处理这个问题。将一块硅胶遥控飞机燃油管套在子弹上，然后将辅助手夹在管子上。这根管子将作为子弹和弹夹之间的绝缘层。硅树脂很容易承受焊接的温度。我还在钳口上使用了硅胶管——尽管最终钳口会切断软管。

这一版就这么多啰嗦！直到下一次，让他们飞起来！

标题照片信用赛勒斯阿卜杜拉希。