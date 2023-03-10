# 如何建立一个代理汉姆尽管取消了 DEFCON 会谈

> 原文：<https://hackaday.com/2015/07/14/how-to-build-a-proxyham-despite-a-cancelled-defcon-talk/>

几天前，Rhino Security 的本·考迪尔(Ben Caudill)计划在 DEFCON 上发表演讲。他的项目 ProxyHam 是为那些寻求完全匿名上网的人设计的。因为 IP 地址可以与物理位置联系在一起，任何在线活动都可以被暴虐的政权和三信政府机构跟踪。有时，这意味着大门被打破，而“煽动性”的记者和活动家被拘留。

使用 ProxyHam，IP 地址和物理位置之间的链接被切断。ProxyHam 使用 900MHz 无线电链路来桥接数英里以外的 WiFi 网络。通过在有公共 WiFi 的空间隐藏一个 ProxyHam 基站，任何人都可以在线完全匿名；如果政府来抓你，他们首先得在当地图书馆、星巴克或者任何有免费 WiFi 的地方停下来。

[【本·考迪尔】将不会在 DEFCON](https://www.defcon.org/html/defcon-23/dc-23-speakers.html#Caudill) 上发表演讲。取消演讲不是 DEFCON 组织者的选择，也不是他的雇主——[Ben]创建了 Rhino Security，并且是它的首席顾问。[被杀了，没人知道为什么](http://arstechnica.com/security/2015/07/a-200-privacy-device-has-been-killed-and-no-one-knows-why/)。猜测的范围从国家安全信件到政府的禁言令，再到更加平淡的解释，比如“它没有像预期的那样工作。”然而，关于为什么 ProxyHam 会谈被取消的细节将永远不得而知。这并不意味着这种知识丢失了——你可以用从亚马逊、新蛋或许多在线零售商中的任何一家购买的设备建立一个 ProxyHam。

### 如何构建 ProxyHam

![Image from the original Wired Announcement](img/63de2e2985ba9ac1db3c8f829e0c484a.png)

Image from the original [Wired Announcement](http://www.wired.com/2015/07/online-anonymity-box-puts-mile-away-ip-address/)

[在 *Wired* 的文章中，鼓吹着世界的临近](http://www.wired.com/2015/07/online-anonymity-box-puts-mile-away-ip-address/)，【Ben Caudill】拿着一台笔记本电脑，连接到一个装有相当大的八木天线的小盒子上。这根天线指向地平线上方，表明该设备没有被使用，但这完全是题外话。ProxyHam 盒子里有一个东西，一端是 RJ45 连接器，另一端是两个射频连接器。快速浏览新蛋[登陆这个](http://www.newegg.com/Product/Product.aspx?Item=9SIA1EA0CD6562)，这是一个无线电基站，旨在通过 900MHz 无线电桥接网络。你需要买两个来复制 ProxyHam。

*Wired* 的文章进一步描述了 ProxyHam 一台连接到 Wi-Fi 卡的树莓 Pi 计算机和一个小型 900 兆赫兹天线…”新蛋还储备了[树莓 Pi](http://www.newegg.com/Product/Product.aspx?Item=9SIA4642TT8991)、[天线](http://www.newegg.com/Product/Product.aspx?Item=N82E16815670028&cm_re=antenna_900MHz-_-15-670-028-_-Product)和 [WiFi 适配器](http://www.newegg.com/Product/Product.aspx?Item=N82E16833315091)。你可能也想买几张 SD 卡。

![900MHz router seen in the original promo image](img/aaa318163cbad7a5c6bd4cbf77e8e360.png)

900MHz router seen in the original promo image

要设置 ProxyHam 的“一次性”部分，您需要首先连接到所需的 WiFi 网络，然后桥接 WiFi 和有线连接。用 Raspberry Pi 搭建网络是留给有足够 Google-fu 的读者的一个练习。当然，900MHz 基站也必须进行配置，但根据 [Ubiquiti 产品页面](https://www.ubnt.com/airmax/rocketm/)上的用户指南，这并不比配置 WiFi 路由器难多少。将收音机设置为“桥接”模式。

从那里，这是一个简单的问题，连接一个大型八木天线到 ProxyHam 的“移动”部分。以下是你如何建造一个。配置基站，并将以太网电缆插入笔记本电脑。恭喜你，你刚刚从新蛋买了东西，复制了一个在 DEFCON 上的演讲。

这就是如何构建 ProxyHam 的方法。这也是违反 FCC 第 97 部分禁止加密的方法——你不能在业余无线电上使用 SSH 或 HTTPS。这也是你如何被指控计算机欺诈和滥用法案；从几英里外连接到图书馆的 WiFi 肯定是“超出授权访问”

不要尝试此版本。不合法，很傻，反正 900MHz 频段都被淹没了。此外，如果你的匿名上网计划围绕着从星巴克偷 WiFi，为什么不直接从街对面的麦当劳偷呢？

### 让我们推测一下为什么 ProxyHam 会谈被取消了

现在是七月。几周后，黑帽安全会议将在拉斯维加斯召开。一周后，防御战将开始。这是“安全专家”推销自己、向一些科技记者通风报信、利用阿拉伯之春并为自己扬名的黄金时间。这每年都会发生。

ProxyHam 因为一封国家安全信件而被取消的想法是荒谬的。该版本按照设计的方式使用现成的组件。这违反了计算机欺诈和滥用法案，并且在无线电上使用加密违反了联邦通信委员会的规定。这是违法的，这会让你受到一些联邦指控，但用鞭炮炸邮箱也是违法的。

如果你认为联邦调查局和其他邪恶的政府力量没有能力对本·考迪尔和代理汉姆采取行动，你就不必担心政府的监视。你所看到的只是一年一度的网络安全马戏，它只不过是一场表演。

ProxyHam 是今年的 BlackHat 和 DEFCON 赛前赛。一个有点意思的安全漏洞被提供给科技媒体，然后被吞噬。这成为研究人员简历上的一个亮点，如果这些卡成功，他们每小时可以收取更多费用。研究人员有动机在 DEFCON 上发表最有新闻价值的演讲，这意味着一些演讲者不是在玩安全游戏，而是在玩公关游戏。

十有八九，[本·考迪尔]只是想出了一个办法来保证他拥有 DEFCON 上最受关注的研究员。你所需要做的就是取消谈话，让技术记者推测国家安全信件和政府最高层对出版 ProxyHam 的反对意见。

仔细想想，其实有点印象深刻。本·考迪尔用一些路由器和一个树莓 Pi 黑进了媒体。如果这都不值得尊重，那就没什么值得了。