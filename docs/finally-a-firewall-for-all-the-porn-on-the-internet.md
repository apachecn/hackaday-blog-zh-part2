# 最后，为互联网上的所有色情内容设置防火墙

> 原文：<https://hackaday.com/2013/07/29/finally-a-firewall-for-all-the-porn-on-the-internet/>

![porn](img/41e97c9e985bd89e5d5079431e09144f.png)

现任英国政府正在提议建立一个互联网色情防火墙。与朝鲜、中国、伊朗、沙特阿拉伯和叙利亚等其他拥有互联网防火墙的国家不同，英国公民非常乐于助人[他们中的一些人决定帮助编写新的色情过滤器](http://sicksad.com/blog/2013/07/28/dont-worry-government/)。色情防火长城背后的想法很简单:如果用户想访问 NSFW 网站，就让他们去吧。如果用户想访问互联网的其他 19%,屏蔽它，并把它们转发到一个以手绘 cockswains a baubles 为背景的页面。

防火墙的工作方式实际上非常聪明——它根据 OpenDNS FamilyShield 过滤器检查每个请求。如果请求被拒绝，加载页面，如果 OpenDNS 请求被允许，阻塞页面。

这个过滤器背后的天才，[sicksad]提供了让你自己的色情过滤器在他的 git 上运行所需的所有工具。下面还有一个很棒的安装教程视频，还有一些免费的社会评论。

[https://www.youtube.com/embed/xJfyNwM6Lw8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/xJfyNwM6Lw8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)