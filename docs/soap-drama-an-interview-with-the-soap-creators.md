# 肥皂剧:对肥皂剧创作者的采访

> 原文：<https://hackaday.com/2014/03/11/soap-drama-an-interview-with-the-soap-creators/>

几天前，[我们听到了 SOAP](http://hackaday.com/2014/03/07/soap-the-home-automation-router-and-kickstarter-scam/) 的风声，这是一个基于 Android 的家庭自动化路由器的 Kickstarter 项目。四核 ARM、四个千兆以太网端口、802.11ac、SATA 和世界上所有的收音机——所有这些都只需 100 美元(无显示屏，带显示屏 170 美元)，这似乎好得难以置信。当时，情况可能是这样的:PCB 原型中的图像来自[Bunnie Huang]的开源笔记本电脑，没有足够的以太网端口来连接路由器，硬件看起来完全不对劲。

SOAP 背后的家伙们已经决定通过在他们的 Kickstarter 页面上发布[一个巨大的更新并回答我的几个问题来回应这些指控。采访如下。](https://www.kickstarter.com/projects/soaprouter/soap-first-smart-router-w-touch-display-powered-by/posts/773725)

* * *

**HaD:**[有一个基本包(SOAP sans display)的 BOM/成本分析明细](https://www.kickstarter.com/projects/soaprouter/soap-first-smart-router-w-touch-display-powered-by/comments?cursor=6033963#comment-6033962)，总成本约为 130 美元。这是认捐 100 美元的奖励。这种成本分析有多准确，你打算如何达到这个回报水平？

你提到的这个成本分析非常准确。我们不会从早期发布的 60.00 美元的定价中获利，我们已经采取了亏损领先的定价来吸引支持者和媒体(我们认为我们已经做得很好了)。我们正在与一家大型路由器制造商合作，这确实是使定价成为可能的纽带，没有他们我们无法做到这一点。

**HaD:** 您将四核 Freescale i.MX 处理器用于 SOAP，并在其中放置了一个四端口千兆路由器。[四核 i.MX 芯片](http://www.freescale.com/webapp/sps/site/prod_summary.jsp?code=i.MX6Q&nodeId=018rH3ZrDRB24A&tab=Buy_Parametric_Tab&fromSearch=false)只有一个千兆端口[，而且仅限于 470 Mbps](http://hackaday.com/2014/03/07/soap-the-home-automation-router-and-kickstarter-scam/?preview=true&preview_id=116659&preview_nonce=7f710b7ad2) 。你是如何解决这个问题的，你用什么作为 MAC/PHY？

SOAP: 首先让我声明，我们非常清楚 CPU 的局限性，我们已经做了大量工作来寻找解决方案，我们确实有一个独特的解决方案。我们得到了路由器行业一家大型企业的支持，该企业为我们提供了一个独特的解决方案，我们一直在努力解决这个问题。在我们的圣何塞之旅之后，我们将会发布更多的内容。这是我们的后备方法，是的，它的基准没有我们想要的那么好，但是他们正在达到目标，我们觉得通过足够的调整，我们可以达到一个不错的水平。

这是来自我们的设计人员:我们计划将 I.mx 处理器的千兆位端口连接到外部 IC，作为一个开关。1Gb 以太网-> 1 到 4 个交换机-> 4x Gb 以太网端口。可能的 http://www.ti.com/lit/ds/symlink/tnetx4090.pdf。使用 4 个端口，每个以太网端口使用 Marvell 的 RGMII 以太网收发器，我们将有板载以太网交换机。

**HaD:** 您使用的是什么 WiFi 芯片组？他们能够全速运行 802.11ac 吗？在更新的主板图像上，你们(我认为)只有一根天线是如何做到的？

**SOAP:** 芯片组的速度变化很大，软件当时也有很多问题，但我们的时钟速度超过了每秒 1 千兆字节，我们将继续进一步发展，以实现最大速度，这就是我们与 Droidifi 的家伙们的新联盟将提供帮助的地方。

在我们的样机中，我们测试了 [Avastar 88W8864](http://www.marvell.com/wireless/avastar/88W8864/) 、Broadcom [4360](http://www.broadcom.com/products/Wireless-LAN/802.11-Wireless-LAN-Solutions/BCM4360) 以及几个实际上无法工作的产品。我们没有得到我们想要的所有功能，因为到目前为止对 android 和路由器芯片组的支持很少。我们使用 Broadcom 芯片组进行演示。

我们希望使用 Quantenna QAC2300，但在目前的资金情况下，我们将使用 Broadcom。我们收到了来自我们的支持者和我们背后的一家新的大公司的许多建议，他们认为他们有合适的匹配。我们正在等待在圣何塞会议后宣布这一点。

在最新的设计中，我们有一个天线，但我们计划在最终设计中增加两个天线。我们没有把它们放在最新的设计上，因为我们在等着看我们得到多少资金来完成 wifi 芯片组。当我们转向漫威或 Quantenna 时，我们不希望天线设计与 Broadcom 配合得最好。

**HaD:** 软件的状态如何？你有一个回购的地方，人们可以看看吗？

SOAP: 我们一直在与旧的 kickstarter 项目 Droidifi 中的一个新玩家合作。我们将和他们一起开发软件。这是我们在封锁之前无法宣布的事情，但是你是第一个知道这个联盟的人。今天晚些时候看看我们的更新。

 ****HaD:** 最后，你有没有一个四核 i.MX、四个以太网端口和 WiFi 的功能原型？我们能看视频吗？

SOAP: 如果你指的是最终用户可以使用的大规模生产设备，那么不是。我们有一个可靠的功能性概念验证原型。我们有很多概念验证的演示视频，展示了我们到目前为止所开发的内容。我们必须制造当前的 PCB 设计，以便进行更严格的测试和认证。我们 kickstarter 上列出的所有规格都是我们目前正在计划的，我们希望能够实现这些技术规格。

在 Kickstarter 评论区有一些其他的问题，但老实说，我不在乎你有多少 Twitter 粉丝。

SOAP: Twitter 是我们的营销公司。我们以为人们真的在跟踪我们，但后来我们发现其中一半不是真的。不过检查一下[这个](http://www.dailymail.co.uk/news/article-2430875/Barack-Obama-19-5m-fake-Twitter-followers.html)出来。

总之，我们知道这个项目看起来有多么雄心勃勃，我们也知道 it 技术发展可能会遇到障碍和问题，但我们希望明确我们不是一个骗局，我们非常清楚这些攻击来自哪里。我们将继续在这个项目上努力工作，我们不会跑到哥斯达黎加，我们计划在明年的 CES 上见到大家。

* * *

#### TL；针对所有注意力不集中的人的灾难恢复:

是的，100 美元/170 美元的价格好得令人难以置信。这叫赔本赚吆喝。这部分是成功的。SOAP 人员正在与 DroidFi 人员合作开发操作系统。千兆以太网可能会工作，WiFi 受到*nix 芯片组支持的限制。还没有完整的功能原型。

所以你走吧。SOAP 工作人员展示了一个准备发货的单元集装箱，这不是一个理想的更新，但是这个项目并不像我最初想象的那样糟糕。**