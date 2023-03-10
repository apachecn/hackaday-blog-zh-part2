# 一种不同类型的 Arduino 互联网盾

> 原文：<https://hackaday.com/2013/07/12/a-different-type-of-arduino-internet-shield/>

![different-arduino-internet-shield](img/c82661e540f714cebaff034b8990600b.png)

Arduino 的以太网屏蔽的成本并不可怕；一般在 17 美元到 32 美元之间，取决于你买的是哪一种。但是你见过一个 WiFi 盾的成本吗？那些已经超过 70 美元了！[Martin Melchior]提供了一种解决方案，可以让您选择低成本的以太网或 WiFi，并且适用于大多数应用。他使用 WiFi 路由器作为 Arduino 互联网屏障。

这是 TP-Link WR703N，它非常受黑客的欢迎，因为它结合了低价格(很容易找到，价格为 25 美元或更低)和许多功能:USB 是超级手，嗯，它是一个 WiFi 路由器！Arduino Pro Mini 显示的死错误样式正在使用其串行端口与路由器对话。[Martin]将一个插脚插座连接到路由器上，这样剩下的组装就像将两者插在一起一样简单。他的文章的其余部分讨论了用 Arduino 代码处理双向通信。

如果你真的只需要直接以太网管道，考虑在你的设计中内置一个 ENC28J60 芯片。