# 摆弄朝鲜的网络浏览器 Naenara

> 原文：<https://hackaday.com/2015/01/10/messing-around-with-naenara-north-koreas-web-browser/>

为了更多地了解朝鲜的内部网是如何工作的，罗伯特一直在奈那拉四处打探。 [Naenara](http://en.wikipedia.org/wiki/Naenara "Naenara") 是与朝鲜官方基于 Linux 的操作系统[红星操作系统](http://en.wikipedia.org/wiki/Red_Star_OS "Red Star OS")捆绑在一起的网络浏览器。[Robert]曾经看过一个浏览器的截图，觉得很有意思的是，浏览器好像一启动就自动加载了一个不可路由的 IP 地址。这让他好奇人们可能会从软件中发现什么其他奇怪的东西。

启动时，浏览器会尝试加载一个位于 IP 地址 10.76.1.11 的页面，这是一个专用的保留 IP 地址。这表明朝鲜的“互联网”实际上更多的是在内部网。[Robert]怀疑整个国家可能都在私有地址空间中运行，类似于您的家庭或企业的运行方式。

[Robert 的]下一个想法是，该浏览器看起来像一个非常旧的 Mozilla Firefox 版本，但在默认配置上有一些变化。首先，所有的崩溃都会自动传递到[罗伯特]称之为“母舰”的地方。他怀疑这不仅是为了修复漏洞，也是为了发现和修复任何可能让用户获得更多控制权的安全漏洞。

还有一些其他有趣的变化，比如支持的安全证书。Naenara 浏览器只接受朝鲜颁发的证书，这将使他们很容易窥探加密的 HTTPS 流量。还有证据表明，整个国家的所有流量都通过一个政府控制的代理服务器进行路由。

这些发现都不令人惊讶，但看看从浏览器和操作系统中能发现什么样的信息还是很有趣的。[罗伯特]发现的不仅仅是这些发现。你可以在他的博客上查看他的其他发现。

[via [Reddit](http://www.reddit.com/r/netsec/comments/2rsisc/north_koreas_naenara_web_browser_its_weirder_than/ "Reddit.com")