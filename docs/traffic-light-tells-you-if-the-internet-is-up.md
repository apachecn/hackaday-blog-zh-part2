# 交通灯告诉你互联网是否开通

> 原文：<https://hackaday.com/2015/09/12/traffic-light-tells-you-if-the-internet-is-up/>

我们中的一些人没有一个永远在线的、高可用性的互联网连接。厌倦了不断地回答“互联网开通了吗？”问题、IT 支持 dude [PatH]亲自动手，为他明显不太可靠的连接开发了一个[不会出错的互联网状态红绿灯显示](http://whiskeytangohotel.com/internetup)。

亚马逊的一个玩具交通灯构成了 UI 的核心，灯由树莓 Pi 驱动，它以循环方式 pings 一组 10 个站点。如果发现一个站点不可用，Pi 将进入“深度探测”模式，以确定中断的程度，并相应地亮起。如果灯是绿色的，连接是干净的；如果红灯亮了，最好去睡觉。额外的好处是，所有深度探测都有日志记录，这对于诊断 ISP 问题可能很有用。

像这样的显示器可以大大有助于确保您保持联系，并可以减少您作为事实上的 IT 支持的工作量。当然，关于复古风格的连接速度的更多信息，[你可能想在工作中使用 Dekatron](http://hackaday.com/2015/07/30/an-internet-speedometer-with-a-dekatron/)。