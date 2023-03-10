# 瓶子里的圣诞灯和船

> 原文：<https://hackaday.com/2014/12/01/christmas-lights-and-ships-in-a-bottle/>

感恩节是上周，圣诞节已经入侵百货商店两三个月了，这只能意味着一件事:是时候杀死一棵树，把它放在你的客厅里，并在上面放上几百瓦的灯。所有那些灯，虽然；这就好像圣诞灯是专门为单口相声演员发明的，一年中有两个月是这样。为什么不能有人发明*无线*圣诞灯？

我们不知道它是否已经被发明出来，[但这里有一个 Kickstarter 的活动，正在推销同样的想法](https://www.kickstarter.com/projects/1034423012/aura-the-first-ever-wirelessly-powered-christmas-l)。它被称为 Aura，就像罐头上写的那样:无线圣诞灯，可以用智能手机控制。如果可行，这是个绝妙的主意。

以下是 Aura 的基本技术分析。一堆带有大线圈和发光二极管(几乎没有其他东西)的印刷电路板不知何故被塞进了玻璃球饰品中。这些装饰品通过射频供电，射频由一个线圈提供，线圈卡在树上，插在墙上。这种线圈能够为 5 英尺外的灯供电。对于高于五英尺的树，您可以在树的中间折断线圈。一个线圈可以为大约 100 盏灯供电。智能手机的“调度”直接在线圈上完成，打开或关闭所有的灯，所以不用担心将 WiFi 放在几十个玻璃球中的疯狂电力需求。

在我看来，像这样的东西肯定是存在的。每个装饰品中的 led 消耗的能量很小，因为你可以用 Powermat 或其他无线充电器给手机充电，所以即使考虑平方反比定律，你也可以用一个真正大的“电源环”给几个 led 供电。EMC 测试完全是另一回事，但至少是可能的。

然而——总有一个“然而”——关于这个的一些东西没有通过嗅探测试。我花了一段时间看 Kickstarter 活动，直到我抓住它，现在我有一些无法回答的问题。他们到底是怎么把 PCB 放进玻璃球里的？是的，这是经典的瓶中船问题，只是你不能在玻璃球中组装 PCB。

那些也不是塑料球。光环的创造者明确表示他们是玻璃:

> 我们试验过的塑料手机实际上非常酷，只是没有干净的玻璃手机那么“优雅”，这就是我们没有从那里开始的原因…因为这是一种全新的技术、想法和实施，我们需要专注于交付，因此目前只有一部分可用的选项。

每天查看几十个可疑的 Kickstarters 是一件奇怪的事情。大多数项目都很容易理解，你可以很快对一个项目的可行性和潜在的成功做出判断。很少，你会看着一个项目，一些看似无关紧要的东西会抓住你的眼睛。一个很好的例子[是将一个芯片放入一个太小的外壳](http://hackaday.com/2014/08/14/scribble-wait-kickstarter-is-vetting-projects-now/)——一个相当无关紧要的细节，就像拉一根松了的线，解开了整个活动。

我们现在有了光环，一些可能的东西，但在我的脑海里有一个没有答案的问题。所以我们去寻找更多。

这里有一个来自 Aura 运动的视频，它是如此的甜，以至于会让诺曼·洛克威尔患上糖尿病。这正是你在 Kickstarter 视频中想要的:不要展示产品，只展示有了产品你的生活*会变得多好。这个视频唯一的画外音是，“在你的世界里有很多第一次。你的第一步。你的第一个圣诞节。现在，有史以来第一个无线圣诞灯。”我们迫切需要媒体理论家开始搜索 Kickstarter 视频。*

[https://www.youtube.com/embed/cS5CPuxez_I?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/cS5CPuxez_I?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

很平淡，是吧。让我们来看看这段视频中的两个画面。第一帧显示一个男孩把一个透明的玻璃装饰品放在树上。要特别注意，因为这个装饰品里面没有任何东西。

![lol](img/b8a681a9d3fecc29fe48b441e790958f.png)

仅仅几秒钟后，通过圣诞精神的力量和一个你可以在 Kickstarter 上花 69 美元购买的设备，装饰品神奇地亮了起来:

![wut](img/52c7e7a616a1bf312e12e618ca0df16c.png)

一个美丽的家庭聚会，一个光影的相互作用，一个很好的证据，来自装饰品的光是后期添加的。仔细看最后一幅画，你就会明白它是怎么做的。一个点被放置在右边；半棵树从错误的方向被照亮。索尼维加斯或最终剪辑的一点点照顾到实际的装饰品照明-如果这个词是一个形容词，从装饰品发出的光太高斯了。事实上，所有关于照明的争论都是没有实际意义的，因为我们已经知道一开始装饰品里就没有任何东西。

我不干了。看到这个之后，我真的不能再评价 Aura 了。Aura 团队正在展示一个显然是伪造的视频，作为一个真正的无线圣诞灯。我想不通他们是怎么把 PCB 装进玻璃球里的。我甚至不想去分析这种说法，“能量环安全地产生了一个磁场，只有当接收器进入它的磁场时才传输能量。”当然，这就是你的用武之地。欢迎评论，伙计们。让我们听听你的看法。