# 交通灯袖扣

> 原文：<https://hackaday.com/2012/10/17/traffic-light-cufflinks/>

![](img/cbd0c0fbf335dcc672753912cffea541.png "traffic-light-cuff-links")

[Brendan Sleight]一直在努力开发这种可穿戴技术。他不怎么戴珠宝，但一枚结婚戒指和一些袖扣是他外表的一部分。为了增加一些极客，他设计了一套袖扣，功能就像交通灯一样。因为他还有一些剩余的程序空间，他还加入了额外的功能来配合交通灯的显示。

该链接指向他的工作原型帖子，但是您可能想四处看看，因为他的帖子中充斥着来自开发过程每个部分的信息。隐藏在外壳内的硬币大小的 PCB 充当红色、琥珀色和绿色表面贴装 LED 的主机。在它们的两边，你会发现一辆 ATtiny45 和一辆 RV-8564-C2。后者是集成晶体振荡器的表面贴装 RTC，非常适合空间非常紧张的项目。

该设计将外壳用作触摸传感器。每隔几秒钟，ATtiny 就会醒来，查看链接是否被触动。这可以确保硬币电池不会因为持续驱动 led 而耗尽电量。触摸式菜单系统让你可以像停车灯一样运行链接，或者显示时间、日期或当前温度。休息之后，请观看快速演示剪辑。

[https://www.youtube.com/embed/GpnWxmfzyew?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/GpnWxmfzyew?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)