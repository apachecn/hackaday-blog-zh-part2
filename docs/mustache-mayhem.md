# 八字胡任天堂虚拟男孩去增强现实

> 原文：<https://hackaday.com/2015/03/25/mustache-mayhem/>

有些人只想看着世界燃烧。其他人想要传播和平、快乐和胡子。这一次，乔·格兰德属于后一类人。他的最新作品是[小胡子大混乱](http://www.grandideastudio.com/portfolio/mustache-mayhem/)，集黑客、视频游戏和艺术项目于一身。这与[拆解电路板](http://hackaday.com/2015/03/05/deconstructing-pcbs/)或设计电子徽章有所不同，但对于【乔】来说并不完全是新的，他在 2000 年初为雅达利 2600 编写了[SCS cidice 和 Ultra SCS cidice](http://www.grandideastudio.com/portfolio/scsicide/)

小胡子大混乱是一个任天堂的虚拟男孩住宅。虚拟男孩本身就坏掉了，不幸的是无法修复。[Joe]移除了大多数库存电子设备，并添加了 BeagleBone Black、Logitech C920 网络摄像头、LCD 屏幕和一些定制电子设备。他保留了原来的音频放大器、扬声器和控制器连接器。Angstrom Linux 启动到[Joe 的]软件，该软件使用 OpenCV 来检测面部并覆盖胡须。游戏很简单:将控制台指向一张或多张脸。如果你看到小胡子，按控制器上的 A 按钮！屏幕上一次出现的面孔和胡子越多，玩家得到的点数或“魔力”就越多。代码在 [Github](https://github.com/joegrand/mustache-mayhem) 上，可以用针对 Mac 的 Xcode 构建，或者直接在 BeagleBone Black 上构建。

[Joe]该项目的目标是制作一个荒谬的游戏，看起来像是在 90 年代问世的。他还将小胡子混乱作为一种有趣的方式来学习一些新技能，这些技能将在未来更严肃的项目中派上用场。

我们采访了[Joe],对他的新作品进行了简短的采访。

你是如何想出小胡子混乱这个主意的？

几年前，我在 PRGE (Portland Retro Gaming Expo)出售一批我收集的电子游戏，有一个坏掉的虚拟男孩，但没人买。我的一个朋友坐在桌子旁边，说我必须做点什么。我想“人们穿着 cosplay，在会议上走来走去，那么如果我能和你可以一起走的虚拟男孩做些什么呢？”那是种子。

几个月后，德州仪器给我发来了 BeagleBone Black 的原始生产版本(版本 A5A)。18 个月后，我实际上开始了这个项目。催化剂是为即将到来的波特兰艺术展(Byte Me 4.0)做点什么，这是一个展示基于互动技术的艺术品的年度活动。我写了一点描述，然后被录取了。我只有不到两个月的时间让事情运转起来，结果花了大约一个月的全职工作。对于这样一个愚蠢的项目，这比我预想的要多得多。我原本打算做一些类似末日视角的东西，当人们的脸被检测到时就拍摄他们。

那会非常酷。你是怎么从厄运变成大胡子的？

我看到了一个 TI 猎兔犬演示，名为“ [boothstache](https://github.com/misterbonnie/stache) ”，它在脸上画了胡子，并在推特上发布了照片。我认为留胡子做一些非暴力的事情更适合(也更有趣)给我的孩子们看。我还偷偷想把这个项目作为一种尝试 Linux 的方式，编写一些代码，并学习 OpenCV 的人脸检测和图像处理，我计划在未来用于一些实际的计算机安全研究。小胡子大混乱变成了一个超级酷的项目，我真的很高兴。在它上面花了这么多时间，我有点内疚，因为它基本上只是一个一次性的原型，但我只是太沉迷于按照我想要的那样制作它。

你在自己的网站上提到，小胡子“旨在挑战个人隐私和娱乐的范式”你到底是什么意思？

许多人在网上发布自己的照片(以及各种其他个人身份信息)而不考虑后果。我注意到玩家们愿意把他们的脸放在摄像机前，看看他们有了“虚拟胡子”会是什么样子。我真的不能责怪他们，因为胡子很酷，但如果我可以使用单板 Linux 机器来检测人脸，想想城市，州和民族国家可以在更大的范围内做什么/正在做什么。这种说法是一种潜在的主题，让人们更仔细地思考他们的个人隐私，以及如何以娱乐的名义牺牲它是好还是不好。

项目中你最喜欢的部分是什么？

我喜欢能够创造我想创造的任何东西的自由，只是为了好玩。我对复古/经典游戏有一种真正的亲近感，所以尝试让游戏看起来像是属于 90 年代的(虚拟男孩最初发布的时候)很有趣。能够使用股票虚拟男孩控制器是另一个亮点，因为它使游戏看起来更完整，更少的黑客(从外表看)。

你必须从头开始制定协议吗？

不，这节省了我很多时间。我在网上找到了一个关于虚拟男孩控制器引脚和接口的文档，所以我把它作为一个起点。编写与控制器通信的代码并没有花很长时间(它使用同步串行接口，基本上只是移出一串位，每个位对应控制器上的一个按钮)。

你遇到什么意想不到的挑战了吗？

这是我第一次真正深入地使用 Linux。我遇到了各种各样的麻烦，包括配置系统、编译各种包，以及强迫它做我想让它做的事情。这纯粹是我自身技能的局限。如果没有 Linux 和 BeagleBone Black 的大量开源工具和资源，我可能会彻底完蛋。我是一个硬件专家，所以这是一次真正的考验。

一个更大的意想不到的挑战是意识到我选择的电池(Energizer L91 锂 AA 原电池)无法满足系统的功率要求(约 7W)。这是我的一个重大疏忽，直到艺术展开幕之夜，我才注意到这个问题，当时我开始看到这个装置似乎被随意关闭了。我简直不敢相信自己的眼睛。这就像一个噩梦，让我想起了拍摄原型时的压力，当时摄像机在转动，每个人都在看着你。

你是如何为这部剧找到灵感的？

我以为电池快没电了(从技术上来说，确实如此)，所以我改用了库存的虚拟男孩墙疣。我不知道，这也是我的设计动力不足。那天晚上，系统关闭了两次，但幸运的是，与会者仍然体验了小胡子混乱的奇迹。

演出结束后，我找出了问题的根源:当使用电池运行时(虚拟男孩控制器使用六个串联的 aa)，系统电压在游戏开始前就已经下降到 7V(从标称的 10.2V)。我一启动游戏(启用了网络摄像头)，电压就降到了我的 DC/DC 转换器的 7V 最低限值以下，导致系统关闭。使用壁式电源(10V，850mA)时，它在负载下的输出实际上是一个三角形(！)挥手。有时，这也会导致 DC/DC 转换器关闭。令人惊奇的是在这个过程中没有任何东西被损坏。在我开发的大部分时间里，我都插着 USB 接口(用于从我的电脑上通过网络访问 BeagleBone Black)，这是对主电源的补充，所以我从未注意到壁灯和电池的糟糕性能。

我最终破解了虚拟男孩交流适配器包(连接到虚拟男孩控制器的背面)，以适应一个标准的 2.1 毫米桶形插孔，并使用了高质量的 CUI 12V，2.5A 电源。负载下的输出完全干净和稳定，没有任何噪音。我无法在 AA 封装(或可以放入 Virtual Boy 电池盒空间的封装)中找到任何可以处理系统高电流消耗同时保持在 7V 以上的电池化学物质，也不想将我的 DC/DC 转换器换成最低输入电压更低的转换器。所以，现在，我只能用墙上的电源。不过，我没意见。

我们要感谢[Joe]抽出时间与我们交谈。我们不知道他下一步会做什么，但我们确信这将是一个伟大的想法！

[https://www.youtube.com/embed/Efp4izKksvY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/Efp4izKksvY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)