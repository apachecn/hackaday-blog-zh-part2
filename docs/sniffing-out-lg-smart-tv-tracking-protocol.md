# 嗅出 LG 智能电视跟踪协议

> 原文：<https://hackaday.com/2013/11/23/sniffing-out-lg-smart-tv-tracking-protocol/>

[doctor bete]注意到了他的新 LG 智能电视登录屏幕上的广告，并开始考虑跟踪。当他看到一个针对广告商的宣传视频，吹嘘从这些电视用户那里收集的信息时，他的好奇心占了上风。他决定嗅探网络流量。如果他的发现是准确的，那么这个硬件正在收集大量的数据。更糟糕的是，他的测试表明，即使用户将“收集观看信息”菜单项关闭，也不会阻止数据被打电话回家。

这些发现开始时相当无害，每次换台时都会传输频道名称和唯一的 ID。根据服务器收到数据包的时间，可以将您的时间表和首选内容放在一起。这似乎是作为普通数据发送，没有任何类型的加密或混淆。

当他发现连接到电视机的 USB 驱动器中的文件名也被广播时，事情变得有趣多了。它们被发送到的服务器地址是一个死链接——这让我们认为这是生产固件中留下的某种类型的调试步骤——但当涉及到个人隐私时，这仍然是一个相当大的错误。如果你有一台这样的电视机，为了保护你的隐私，[doctor bete]会列出一个初步的 URL 列表，用你的路由器屏蔽掉。

[感谢 Radcom]