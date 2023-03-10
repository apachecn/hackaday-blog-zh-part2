# 绕线 101

> 原文：<https://hackaday.com/2014/12/18/wire-wrap-101/>

你可能会注意到我的许多作品都以“回到过去”开始。为了不让人失望，我要说的是，以前当我们需要某种程度上坚固、某种程度上可靠的组件时，我们会使用绕线技术。给定一个可读的原理图，一个好的技术人员可以根据原理图的完整性和准确性在一两天内返回一个工作或接近工作的单元。

[![wire-wrap2](img/3b5eb99c6cb7d86d3f30b12b88ecaadd.png)](https://hackaday.com/wp-content/uploads/2014/12/wire-wrap2.png)

当创建定制 PCB 的替代选项需要太长时间或不允许足够的实验时，正确完成的绕线组件能够具有相当高的速度和可接受的噪声。从电信公司到美国国家航空航天局，绕线也被用于多种类型的产品中，但我完全赞同工程师对此的观点。

我的第一个绕线工具和绕线电线来自 20 世纪 70 年代中期的 Radio Shack。我现在还保留着这条电线，因为坦率地说，它是一种廉价的电线，当我需要在 PCB 上制作跳线时，它是我唯一可以快速找到的东西。该工具仍然在附近，因为我现在找不到它，这里显示的是我的新绕线工具，它适用于少量包装、解包和剥线。

[![ww-tool2](img/365c1b73128d0acd9bf99a9372709868.png)](https://hackaday.com/wp-content/uploads/2014/12/ww-tool2.png) 这个小巧的包裹工具对业余爱好者来说是不错的，因为稍微练习一下包裹就可以了。但是我建议投资高质量的电线。一种常见的电线是 Kynar 涂层，这是一种氟化乙烯，作为绝缘体表现良好。

在我继续深入之前，这里有一个绕线的视频演示，它的用途和几个演示。但是，请务必在休息后加入我，我将向您介绍开始学习绕线大师所需的其余信息。

[https://www.youtube.com/embed/IXvEDM-m9CE?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/IXvEDM-m9CE?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[![wire-spool](img/220b0d1c3511cf2ac3ef3fed3965e9b4.png)](https://hackaday.com/wp-content/uploads/2014/12/wire-spool.png)

另一个重要的你也会听到我竖琴上良好的电源和地面布局；“应尽量减少在终端终止的电源线的短截线或长度，电源线和接地线的布线应相互靠近。将电源和回路电感耦合在一起可降低阻抗，从而降低噪声。很明显还有更多，但这是另一个视频。

良好的缠绕在方形接线柱上有 3-4 匝裸露线，并有一匝绝缘线，可提高对振动和基于振动的故障的抵抗力。这张图来自 NASA 网站的标准部分，显示了一种可接受的包装。

 [![socket](img/39c8c4e1c8b5fc00a060f4f9f97d9842.png "socket")](https://hackaday.com/2014/12/18/wire-wrap-101/socket-2/)  [![sip](img/a3d6c99ff17b732e5775fd9b3630ae1b.png "sip")](https://hackaday.com/2014/12/18/wire-wrap-101/sip-2/) 

线绕插座仍然可用，我保留了线绕 SIP 端子板，因为可以根据需要创建自定义插座。

对于连接器等更复杂的绕线组件，您可能需要寻找其他来源，如电子废品场。Hackaday 的[Brian Benchoff]在[托德·布莱克]的帮助下，从加利福尼亚州太阳谷的 Apex Electronics 获得了一个 64 针“Hershey Bar”绕线插座。

[![Wrap-ID Labels for Wire Wrap](img/bbcd985e35716950f7890405f2bc8488.png)](https://hackaday.com/wp-content/uploads/2014/12/lables1.png)

Wrap-ID Labels for Wire Wrap

标签上的小纸条有助于跟踪从电路板底部看到的“反向”引脚编号。

在接线柱上缠绕导线是通过首先剥去绕线导线上的绝缘层至 1 英寸来实现的。然后将裸线插入绕线工具端的孔中(即中心的**而不是**)，然后将线推入，直到被工具停止。接下来，将工具和电线放置在特定的方形柱上，确保柱进入工具中心的孔中。对于手动刳刨机，该工具用轻微向下的力旋转，以保持电线缠绕紧密，直到电线完全缠绕，在 5-6 圈之间。

对于手动或电动工具，执行相同的程序，将导线插入工具中，然后将工具和导线放置在柱上，最后工具缠绕其设定的圈数。

[![Hand Operated Wire Wrap Gun & Tool](img/06b7fc5c030401b2e7b7d3fcfd6f77cf.png)](https://hackaday.com/wp-content/uploads/2014/12/hand-gun-and-tool.png)

Hand Operated Wire Wrap Gun & Tool

[![Electric Wire Wrap Gun](img/b0e9682887395f85bdb47ff0b143a822.png)](https://hackaday.com/wp-content/uploads/2014/12/electric-gun.png)

Electric Wire Wrap Gun

有不同的技术来组织绕线板上的电线；有时，这些导线一起沿通道走线，有时，单根导线以尽可能短的长度直接穿过电路板。这两种技术各有利弊，因为串扰和阻抗会受到布线位置的影响。

[![header](img/f96e20412c8a4062984eafd2bfd6ea1a.png)](https://hackaday.com/wp-content/uploads/2014/12/header.png)

分立元件可以焊接到接头上，然后插入标准绕线插座，如上图所示，带有 3.3K 电阻。

最后，老莫斯/R&D 准将实验室里的一位名叫[杰夫]的技术员向我展示了他的电路板似乎从来没有太多的松弛。他会拿一个细的绕线工具，装上一个插座销/尾，然后旋转销本身，拉紧松弛部分。虽然这看起来更好，但他没有真正解决的事实是，他在一些导线的末端制作了一个更明显的电感。这种技术以及通道布线技术的答案(技术人员有时会将小束捆扎起来)是，我的电路板将采用“丛林布线”，即引脚之间或多或少的直线连接，松弛问题将通过在两个引脚之间的导线中添加一些回旋来解决，方法是绕过其他引脚，类似于您在高速 PCB 上看到的情况，走线将额外多绕几圈来控制长度/传播时间。

我应该告诉你，有一天[杰夫]扔掉了我的咖啡杯，因为我在里面种了东西。从那天起，直到我离开准将，我每天至少去一趟 R&D 实验室，扔掉他的咖啡杯。

[绕线图来自关于分立布线的[nasa.gov 网站](http://workmanship.nasa.gov/lib/insp/2%20books/links/sections/301_Discrete%20Wiring.html)