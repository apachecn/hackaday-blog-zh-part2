# 制造者集会上的阿达果和 arduino

> 原文：<https://hackaday.com/2015/05/18/adafruit-and-the-arduinos-at-maker-faire/>

Arduino 前线过去几周的明显平静只是海湾地区制造商博览会(BAMF)暴风雨前的平静。宣称 Arduino 名称的两家公司周末都在那里，带着新闻和新产品。讽刺的是，你可以从一个摊位直接看到另一个摊位。世界真小。

或许来自 Arduino LLC 的最大消息是，对黑客友好的 Adafruit 现在将在美国制造官方许可的电路板。与这一消息相竞争的是，Arduino 带来了其新的主板，包括 Yun Mini 和 ARM 驱动的 Arduino 主板。[Massimo Banzi]和 Arduino LLC 似乎正在通过宣布欧洲生产的“Genuino”品牌来绕过 Arduino SRL 商标。欲知详情，请继续阅读！

## 阿达果的联系

正如[Massimo]在他的 BAMF“Arduino 的现状”主题演讲中所宣布的，Arduino 正在授权 [Adafruit](http://www.adafruit.com) 在他们位于纽约的工厂生产一系列“最受欢迎”的 Arduino 主板。因此，那些希望支持 Arduino LLC 购买产品的人也可以同时帮助充实[Ladyada]的腰包。在我们看来，这是一大胜利。

[![CFJ0V-OUMAA4IH_](img/f46227427a7b85c2069b843ddda47e3d.png)](https://hackaday.com/wp-content/uploads/2015/05/cfj0v-oumaa4ih_.jpg)

Photo: Atmel

Adafruit 成为 Arduino.cc 的美国工厂并不完全令人惊讶。自 2005 年成立以来，他们一直在销售电路板并制作丰富的 Arduino 相关教程。最近，Adafruit 与 Arduino LLC 合作创建了 [Gemma](https://www.adafruit.com/products/2470) 板，这基本上是一个基于 ATTiny85 的 Arduino-a-like，在一个小圆形、可穿戴的友好板中。(如果你熟悉 Adafruit 系列，它实际上是 LilyPad Arduino 的圆形小饰品。)

事实上，在交易完成并尘埃落定后，我们有点惊讶的是，这种情况没有更早发生，Adafruit 和 Sparkfun 都在生产授权板，Arduino LLC 正在寻找新的制造商。无论如何，干得好 Adafruit 和 Arduino (LLC)！

## 来自 from Arduino 的(新)硬件

Arduino SRL 有它的 [Yun Mini](http://arduino.org/products/arduino-yun-mini) ，它本质上是 [Yun](http://hackaday.com/2013/09/12/the-arduino-yun-yun-means-cloud/) 的一个较小版本——一个 Arduino Leonardo 与支持 OpenWRT 的路由器芯片组的混搭。我们之前已经[报道过这些](http://hackaday.com/2015/03/12/arduino-v-arduino-part-ii)，但是看到他们本人还是很有趣的。

[![yun_m0_images](img/10f44c818dd6e7f5e52fb7f20201b3f2.png)](https://hackaday.com/wp-content/uploads/2015/05/yun_m0_images.jpg)

M0 很有趣。在问题出现之前，Arduino 用 Atmel 设计了一个基于 ARM-M0+的主板。现在 Arduino LLC 在其网站上将它列为 Arduino Zero T1，但仍然没有出售。Arduino SRL 公司在他们的网站上发布了名为 [Arduino Zero Pro](http://www.arduino.org/products/arduino-zero-pro) 的主板，名称有所不同，但现在该版本被宣传为“M0 Pro”。名称又能代表什么呢不多。电路布局和零件看起来是一样的。

## 门户之战

两家 Arduino 公司都致力于将你的 Arduino 开发引入“云”。(良心迫使我们注意到，“云”实际上只是别人的电脑。)无论如何，这实质上意味着绑定到 web 服务的新的基于 web 和基于浏览器的 IDE 版本。有趣的是，这两家公司对这一点有不同的理解。

根据他们的 Maker Faire 新闻稿，Arduino SRL 将为制造商推出一个门户网站，以“推广和分发他们的产品”，并分享代码和想法。位于[my.arduino.org](http://my.arduino.org)(目前似乎只有密码进入)，这个想法似乎是为基于 Arduino 的产品创建一个迷你 Tindie。这与他们的“Arduino IDE-alpha”相结合，这是一个基于 JavaScript 的 IDE，将在浏览器中运行。

[![Blogpost_f9](img/2f7ce49db75f0f434c455b1333bcc002.png)](https://hackaday.com/wp-content/uploads/2015/05/blogpost_f9.png) 与此同时，Arduino LLC 展示了此前公布的他们的替代开发平台， [Arduino Create](http://blog.arduino.cc/2015/05/05/sneak-peak-arduino-create/) 。Arduino Create 让你可以“直接从浏览器用 Arduino Web 编辑器”编写、编译和上传草图，并将你的代码存储在“Arduino Cloud”中。Arduino Create 看起来很光滑:肯定比我们习惯的普通 Java IDE 好得多。现在说这个“云”是什么还为时过早，但看起来它将包括代码共享、原理图和布线连接存储，以及用户之间的轻松共享。

我们已经在用博客了，Hackaday.io ( [不要脸的塞！](http://hackaday.io))、Github 和其他“云”服务来存储我们的项目和代码，所以我们并不完全确定这些门户产品会带来什么。现在是 2015 年，还有人在为网站上的项目托管空间而苦恼吗？

讽刺的是，我们注意到这两家公司都在为“拥有”Arduino 社区而战，让人们在他们的服务器上托管代码和项目是一个显而易见的策略，而提供基于 web 的 IDE 来促进这种捕获是一种战术。

在我们离开“云”之前，我们应该注意到两个 Arduinos 都迟到了。自 2012 年以来，codebender 已经出现并在网络上编程 [Arduinos。](http://hackaday.com/2012/07/01/codebender-an-online-arduino-ide/)

## 新名字

[![CFJz1PHVEAAUTqo](img/c7fff614322e428b03feb7d7d1703aa0.png)](https://hackaday.com/wp-content/uploads/2015/05/cfjz1phveaautqo.jpg)

Photo: Making Society

最后，似乎 Arduino LLC 和 Arduino SRL 还不够糟糕，[Massimo Banzi]还宣布欧洲市场的授权主板将以新的“Genuino”名称出售。

实际上，这是一个相当谨慎的策略，因为它回避了欧洲商标问题(在他的谈话中[Massimo]称之为“bullsh*t”)，而且是一个可爱的名字。“正版”，懂了吗？

我们的份额？正如[马西莫]在接受《Make》，的视频采访时几乎说的那样，“玫瑰无论叫什么名字，闻起来都一样香。”如果 Arduino LLC 在意大利的商标诉讼中败诉，他们将不被允许销售使用“Arduino”名称的电路板。限制未来损失的最佳方式是趁所有人都在看的时候，现在就做出改变，给市场时间去适应。