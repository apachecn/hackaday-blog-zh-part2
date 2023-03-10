# 对 HDMI 扩展器进行反向工程

> 原文：<https://hackaday.com/2014/01/25/reverse-engineering-an-hdmi-extender/>

有许多设备可以扩展 HDMI over IP。您将视频源连接到发射器，将显示器连接到接收器，并用 CAT5/5e/6 电缆将二者连接起来。这些电缆比 HDMI 电缆便宜得多，并且可以传输更长的距离。

[Daniel]不在乎扩展 HDMI，相反，他想要一个低成本的 HDMI 输入用于他的电脑。采集卡有点贵，所以他决定[逆向工程一个 IP HDMI 扩展器](http://danman.eu/blog/?p=110)。

连接 DVD 播放器和电视后，他启动 Wireshark 并开始嗅探数据包。该设备在两个端口上使用 [IP 多播](http://en.wikipedia.org/wiki/IP_multicast)。其中一个端口具有高比特率，并且包含 JPEG 头。看起来视频流是原始的 [MJPEG](http://en.wikipedia.org/wiki/Motion_JPEG) 数据。

下一步是编写一个监听器，它可以嗅探数据包并将数据放入 JPEG 文件。在处理了一些奇怪的问题后，JPEG 图像可以从远程设备上保存下来。需要更多的代码让计算机启动流，并从第二个端口提取音频。

最终，用低成本设备进行视频捕捉成为可能。[丹尼尔]还在他的文章中提供了一个额外的设备拆卸。