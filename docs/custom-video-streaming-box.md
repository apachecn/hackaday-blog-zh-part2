# 定制视频流盒

> 原文：<https://hackaday.com/2014/10/12/custom-video-streaming-box/>

现在有很多选择可以将视频流传输到你的联网设备上。无论是 Hulu、网飞、Slingbox，还是已故的 Aereo，都不缺少修理电视的方法。然而，[Jaruzel]对这些服务都不满意，想要一个更加定制化的解决方案，所以他用手头的硬件构建了自己的电视流媒体盒子。

[Jaruzel]从名为 SkyTV 的服务中获取电视，但希望能够将其传输到他的平板电脑、笔记本电脑和 XBMC。在翻遍他的零件箱时，他想到了一个用于捕捉电视的 WinTV 调谐器卡和一个迷你 ITX 板来处理一切并通过他的网络传输出去。

一旦电脑被放入定制的外壳中，[Jaruzel]就开始安装 Puppy Linux。他写了一个启动脚本来配置 WinTV 卡，然后启动 VLC 来处理流媒体服务，这使他可以通过 HTTP 在网络上观看电视流。这是一个很棒的技巧，可能对你能找到的任何电视流都有效，即使它只是一个[无线资源](http://hackaday.com/2012/06/15/hdtv-antenna-that-can-hang-in-a-window/)。