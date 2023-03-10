# 逆向工程 Kayak 移动 API

> 原文：<https://hackaday.com/2015/01/03/reverse-engineering-the-kayak-mobile-api/>

旅游元搜索网站 Kayak 显然曾经有一个公共 API，但现在已经不再提供了。我们不能说我们哀悼我们从来不知道的界面的损失。如果你是一个自动搜索完美度假交易的人，还是有希望的。但不管怎样，你会喜欢这个的。[Shubhro Saha]找到了如何访问 Kayak 移动应用程序使用的 API 的方法。我们喜欢他详细描述了如何嗅探应用程序和互联网之间的流量，并理解所发现的内容。

他选择的工具是 Python 包 Mitmproxy。我们没有听说过它，但我们听说过 Wireshark，而且[shahro]认为 Mitmproxy 更适合这种应用。顾名思义，你在你的电脑上设置它，并使用那个盒子的 IP 作为你手机的代理连接。在使用应用程序一段时间后，有足够的数据开始解构应用程序和它通信的远程服务器之间发生的事情。我们可以从中获得很多乐趣，比如看到那些免费应用程序正在向家里发送什么信息，或者在你自己的作品中寻找安全漏洞。

[感谢胡安通过[推特](https://twitter.com/juanantoniobm/status/550962983174963200?s=03)