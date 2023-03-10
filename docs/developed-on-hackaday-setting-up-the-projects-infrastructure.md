# 在 Hackaday 上开发:建立项目的基础设施

> 原文：<https://hackaday.com/2013/12/13/developed-on-hackaday-setting-up-the-projects-infrastructure/>

[![2013-12_Developed_on_Hackaday](img/4126eb698213947e5ac36e95f300751f.png)](http://hackaday.com/wp-content/uploads/2013/12/2013-12_developed_on_hackaday.png)

我们很确定我们的大多数读者现在已经知道了，但是我们还是要告诉你:Hackaday 社区(作者*和*读者)目前正在开发一个[离线密码管理员](http://hackaday.com/2013/12/06/developed-on-hackaday-lets-build-some-hardware/)。在我们的第一个 DoH 系列的第一个帖子中，我们介绍了这个项目，并呼吁贡献者。在评论部分，我们收到了非常有趣的反馈以及许多功能建议，我们在[的第二篇文章](http://hackaday.com/2013/12/09/developed-on-hackaday-first-feedback-from-users/)中做了详细介绍。最后，我们组织了一次投票，让每个人对项目的名称进行投票。

结果出来了:这个项目的名字将会是 mooltipass 。我们最初想到的是“multipass ”,但[asheets]告诉我们，苹果和佳能都申请了这个商标。[Omegacs]随后提出了“mooltipass”作为替代方案，我们对此更感兴趣。几天前，我们成立了一个[谷歌集团](https://groups.google.com/forum/?hl=en#!forum/mooltipass)，已经非常活跃。

社区驱动项目的一个经常被低估的方面是它的基础设施和管理。你能(如何)管理来自全球各地的几十个积极的人来为一个共同的项目工作吗？你如何让社区了解它的最新发展？

由于 Hackaday 社区对在线工具非常满意，我们选择了:

*   github 向公众发布 mooltipass 资源，并用于固件/软件开发
*   dropbox 分享快速变化的机械设计文件
*   trello 讨论具体话题并讲述我们当前的进展
*   谷歌群组进行一般性讨论

Github 是显而易见的选择，因为它是最常用的在线仓库之一。它允许贡献者跟踪文件的变化，并确保他们拥有 mooltipass 项目的最新版本。鉴于机械开发过程与开发固件截然不同，负责外壳设计的贡献者选择了 Dropbox。这是我们设置的 Trello 板的概述:

[![](img/4ed866ceb5acca78008cfd3ced6b83ac.png)](http://hackaday.com/wp-content/uploads/2013/12/trello.png)

特雷罗是[扎克]建议的(谢谢！).它是免费的，非常容易理解，方便项目管理(从目前我们所看到的来看)。我们习惯于在一个专门的邮件列表中讨论与发展相关的问题，然后将具体问题转移到 Trello。

不幸的是，固件开发人员仍然需要等待第一批原型的到来才能开始编码。下周的 Hackaday 上，我们将详细介绍硬件的第一个版本，目前正在我们的 [google group](https://groups.google.com/forum/?hl=en#!forum/mooltipass) 中进行审查。根据我们得到的反馈，v2 可能会非常不同。如果你想参与这个项目，现在还不晚(如果你不是固件开发人员！)，因此您可以通过 mathieu[at]hackaday[dot]com 与我们联系。