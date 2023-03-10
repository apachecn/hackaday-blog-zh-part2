# DEF CON:Proxy ham 的代理

> 原文：<https://hackaday.com/2015/08/07/def-con-the-proxy-for-proxyham/>

两周前，国家安全局令人难以置信的滥用权力的新闻曝光。一次 DEF CON 会谈被取消，人们猜测信息不是免费的。这就是 ProxyHam，一个能让你远离任何追踪你 IP 地址的机构的设备。

当然，正如媒体报道的每一次 DEF CON 谈话一样，ProxyHam 是一个考虑不周的可怕想法。你可以用从 newegg 购买的部件复制它[，尽管使用了高度定向天线，FCC——或任何其他政府机构——仍然可以追踪到你。](http://hackaday.com/2015/07/14/how-to-build-a-proxyham-despite-a-cancelled-defcon-talk/)

Errata Security 的[Dave Maynor]和[Robert Graham]没有就如何使用现成的网络硬件发表演讲，而是在代理 ProxyHam 的 DEF CON 上发表了演讲。他们彻底揭穿了围绕取消 DEF CON talk 的令人愤慨的猜测，并设法推出了一个新版本的无线互联网，这实际上对有安全意识的个人很有用。

勘误表安全谈话中的“揭穿”部分正是任何人所期望的；这个演讲可能被取消了，因为 ProxyHam 的创造者超过了辐射功率限制，FCC 抓住了他，或者仅仅是因为“律师的建议”。没什么大不了的；有人在做非法的事情——通过 ISM 频段加密——而你预期会发生的事情真的发生了。

在过去的两周里，这些人复制了 ProxyHam 版本，但是发现了一些主要的缺点。即使有高度定向的天线，感兴趣的人仍然可以追踪到你。这使得 Errata Security 的人员改进了这个系统。他们设法在两周内完成了这件事。

勘误表的安全性依赖于 JT65A——一种为非常微弱的信号制造的无线电模式——来将信号隐藏在噪底之下。通过在多个通道上复用数据，该系统的带宽与 1999 年的 56kbps 调制解调器相当。这并不多，但它是可能的，使用这个代理为 ProxyHam 超过 20 英里远的地方，你偷 WiFi。这比 ProxyHam 所能做到的要好得多，而且所有的传输都保持在噪声层以下。FCC 和类似装备的机构可能能够找到你，但是没有一个拥有 20 美元 SDR 加密狗的人会。

目前还没有发布，但勘误表安全计划使允许这种多路传输的软件很快可用，并希望很快有一个基于 Raspberry Pi 的硬件解决方案。这是一个无线电代理解决方案，实际上有点安全，不会立即引起 FCC 的愤怒。