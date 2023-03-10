# 你是一片美丽而独特的雪花

> 原文：<https://hackaday.com/2015/07/16/panopticlick-you-are-a-beautiful-and-unique-snowflake/>

我们都喜欢认为自己是独一无二的，但当涉及到保持匿名在线时，这可能不是一个好主意。到目前为止，众所周知，广告公司、三字母机构和“谁知道谁”想知道你访问了哪些网站以及访问频率。持续跟踪 cookies、第三方 cookies 和“like”按钮可以随时跟踪您。

不管出于什么原因，您可能希望匿名浏览，并尝试堵住一些显而易见的身份泄漏源。EFF 和他们的 Panopticlick 项目给你带来了坏消息。

Panopticlick 背后的想法很简单:即使你不接受 cookies，或者如果你禁用了 Flash，或者如果你使用了“安全”浏览器，也要努力找出你的可识别性。为了创建你的浏览器的指纹，Panopticlick 获取你的浏览器放弃的所有其他小的识别信息，并试图将它们拼凑在一起。

有关该项目的完整论述，请参见[本文(PDF)](https://panopticlick.eff.org/browser-uniqueness.pdf) 。这个项目带来的好处是，你的浏览器提供给服务器的信息可以在没有任何 cookies 的情况下识别你的身份。

[![foo](img/e8350921ea35302a0f3d0777dc15a6a4.png)](https://hackaday.com/wp-content/uploads/2015/07/foo3.png) 例如，服务器可以查询你的浏览器支持哪些插件，如果你安装了任何不寻常的插件，你就会被打上指纹。你的浏览器的用户代理字符串通常过于具体，告诉你在哪个操作系统平台上运行哪个浏览器子子子版本。如果你运行的是 Flash，它可以报告你的系统上安装了哪些字体。这些中的任何一种都很容易成为百万分之一的稀有物种。将它们结合在一起(除非它们都高度相关)可以唯一地给你打上指纹。

不一定能赢。如果你禁用了 Flash，远程站点不会得到你的字体列表，但是因为只有五分之一的浏览器运行时禁用了 Flash，所以你还是丢失了两位信息。如果你运行一个“隐私增强”的小众浏览器，你留下独特指纹的机会会大增，除非你也伪造用户代理字符串。

我运行了两次 Panopticlick 实验，一次用的是 Firefox 浏览器，另一次用的是我实际上大部分时间都在使用的一个不知名的浏览器( [dwb](http://portix.bitbucket.org/dwb/) )。Firefox 运行一个 Flash blocker 标准，所以他们没有得到我的字体列表。但是，浏览器插件和相对较新的 Firefox 在 Linux 上的结合让我独树一帜。

对于晦涩的浏览器测试来说，情况甚至更糟。140 万次点击中只有一次使用 dwb，因此这本身就是个坏消息。我还使用 4:3 宽高比的显示器，24 位色深，1280×1024 像素，这显然是 24 分之一的情况。谁知道呢？

[![foo](img/8ba8dea697980566c880dd3b8114a739.png)](https://hackaday.com/wp-content/uploads/2015/07/foo2.png) 最后，我试用了 [Tor 浏览器](https://www.torproject.org/projects/torbrowser.html.en)，它不仅可以通过 [Tor 网络路由你的流量，](https://www.torproject.org/)还可以删除很多关于你会话的具体数据。情况要好得多，使我不再是唯一可识别的:而是千分之一。(显然，很多人在试用 Panopticlick 网站运行的浏览器。)

如果你对在线匿名感兴趣，使用 Tor 之类的东西来隐藏你的 IP 地址并禁用 cookies 是一个好的开始。但是 Panopticlick 指出这可能还不够。做帽子的时候，锡纸的层数再多也不为过。

尝试一下，并在评论中告诉我们你的感受。