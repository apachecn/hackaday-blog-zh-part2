# Hackaday 奖决赛选手:卫星地面站网络

> 原文：<https://hackaday.com/2014/11/07/hackaday-prize-finalist-a-network-of-satellite-ground-stations/>

你可以用遍布全球的传感器网络做一些令人惊讶的事情，这些传感器都连接到互联网上。成千上万的人已经安装了探测闪电的硬件，T2 的 flightaware 向任何愿意收听飞机应答器并将数据发送回服务器的人提供付费服务。作为黑客日奖(hack aday Prize)的五名决赛选手之一，【SatNOGS 背后的人们正在使用同样的众包数据收集来做一些实际上不在这个世界上的事情:收听不断增加的绕地球轨道运行的业余卫星。

每年都有数十颗立方体卫星和其他业余卫星飞行，它们已经成为一种非常受欢迎的太空环境实验方式，让一些崭露头角的工程师在学校开展一个令人敬畏的项目，并测试一些对国家航天局来说太过怪异的技术。把这些鸟中的一只送上来的问题是把数据带回来；一颗卫星一天只会在一个地点的地平线上经过几次，即使这样，每次也只有几分钟。SatNOGS 团队希望通过在全球各地种植接收器，将它们连接到互联网，并有望提供来自数十颗轨道卫星的实时遥测数据，来改变这种情况。

SatNOGS 团队的[Pierros]非常友好地坐下来回答了我们几个关于他参加 Hackaday 奖的问题。这是下面，就在他们的决赛视频之后。一些 SatNOGS 团队也将出席我们的慕尼黑活动，届时我们将宣布获奖者。

[https://www.youtube.com/embed/z92ALYRHOzc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/z92ALYRHOzc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

```
*Are you surprised over the success of your project so far? Distributed
systems like yours are extremely valuable, but they're not as sexy to the
casual observer as 3D printers and electric cars.*
```

最初我们创建这个项目是作为一个开放的地面站来满足我们自己的需要(作为业余卫星观测者)。不过，很快，许多其他人和社区将从开放的地面站网络中受益这一点变得很明显。因此，网络概念在早期成为了 SatNOGS 项目的核心。从那时起，焦点就集中在全球范围的信息技术和它创造的未来的可能性，以及卫星通信的开放理想上。考虑到普通观众，我们对得到的积极回应并不感到惊讶。依靠社区参与和反馈永远是成功的秘诀。这就是强大的催化项目成长和成功的方式。

```
*Of all the finalists, yours is the only one whose ultimate success is a
function of the network effect. Have there been many people offering to
install the hardware and contribute to tracking satellites? How much would
it cost for someone to build a minimal ground station?*
```

到目前为止，我们得到的参与和兴趣令人印象深刻。我们实际上对此感到惊喜。我们的开发过程是开放的(开发者邮件列表),这使得人们能够定制他们的版本(值得注意的是，帝国！).我们已经有来自世界各地的 11 个人建立了他们自己的卫星导航系统(来自美国，希腊，塞浦路斯，西班牙，英国。荷兰和澳大利亚)。有趣的轶事:一名驻扎在南极洲的研究人员联系我们建造一个卫星导航系统，但我们还没有能够解决它的后勤问题:)一个完全运行的卫星导航系统地面站(包括天线、嵌入式 pc、接收硬件和三脚架)的成本不到 300 美元。

```
*Besides putting ground stations in the middle of the ocean, what is the
biggest challenge to getting to the goal of worldwide coverage of LEO and
MSO amateur satellites? What was the biggest challenge in getting to where
you are now?*
```

地球并不完全是温带的。为了实现全球覆盖，卫星将不得不应对不利的环境条件，这将是我们前进的一大挑战。我们已经简单地谈到了这个问题，但我们坚信，一个拥有想法和测试能力的全球社区将帮助我们缓解这个问题。

要达到我们现在所处的位置，最大的挑战是在现有的生态系统中导航，尝试提取最佳实践并重新利用现有协议来实现最终的模块化。我们不得不重新架构、重新编写和重新设计我们最初的许多想法，以达到最佳模块化和与生态系统共存的当前状态。

```
*Are there any amateur satellites that are relying on your project? Have you
been in contact with any groups that would like to use SatNOGS for the majority
of their mission?*
```

鉴于 SatNOGS 网络仍在部署中，我们不希望任何卫星任务在这个阶段只依靠我们。也就是说，我们与现在和未来的任务(如 LambdaSat)进行了几次有希望的接触，以满足他们的通信需求。

```
*From your documentation, a 'parabolic antenna design is in the works.' A
reasonable-sized dish is not easy to build. What's the story with that?*
```

我们的计算表明，考虑到大多数卫星在 LEO 和 MEO S 波段的 TX/RX 特性，我们将能够使用适合当前跟踪器设置的抛物面天线可靠地拾取信号。s 波段 2.4Ghz 的天线其实并不难制造。盘子的横截面，在铝上切割，然后在上面加一层金属网，这是我们目前的想法。我们现在专注于 VHF 和 UHF 波段，但很快会尝试 S 波段。

```
*There are a few amateur satellites going up that will be working on
much higher frequencies than what an RTL-SDR can support. Will you be expanding
the SatNOGS network based on this?*
```

对于高于 1 Ghz 的频率(如 S、Ku、C 或 X 波段)，我们将使用一个与低噪声放大器耦合的下变频器。我们正在试验的 LNB 已经变得越来越便宜，并且可配置以满足我们的需求。从零开始设计和建造 LNB 对未来来说也是一个不错的挑战。使用下变频器可以将频率降至 RTL-SDR 支持的水平，从而扩展卫星导航的功能。

```
Hypothetical, and we’re not going to hold you to whatever answer you give.
You win the grand prize, a trip to space or about $200,000 USD. Which one
to you take, and what is your reasoning for doing so? Since you're the only 
project in the finalists with a huge team, who gets the ride into space if 
you take that route?
```

去太空旅行是我们大多数人童年的梦想。我们对太空的热爱和迷恋是推动我们开始这个项目的首要原因！在考虑奖项时，很难不考虑这一点:)

考虑到所有的事情，我们决定投资 20 万美元回 SatNOGS 将会对太空中的开源硬件、软件和数据产生巨大的影响。选择现金奖将使我们有能力资助世界各地的足够多的 SatNOGS 站实现全球覆盖，进一步研究其他波段的可靠性和扩展，并围绕该项目创建一个具有工具和资源的可靠社区。一个成功的 SatNOGS 项目有能力彻底改变我们对空间通信的看法以及我们如何设计和利用卫星。这种可能性超出了我们童年最疯狂的梦想，这也是我们努力的目标。