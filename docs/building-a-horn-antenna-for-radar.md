# 为雷达制造喇叭天线

> 原文：<https://hackaday.com/2015/03/22/building-a-horn-antenna-for-radar/>

你已经为自己建造了一个很棒的雷达系统，但是它的性能并没有你希望的那么好。你认为这可能与你用来做天线的锡罐有关。显而易见的下一步是设计和制造一个[喇叭天线](http://hforsten.com/horn-antenna-for-radar.html "Building a horn antenna")为你的雷达系统工作。[Henrik]正是以这种方式来改进他的调频连续波[雷达系统](http://hackaday.com/2014/12/03/extremely-detailed-fmcw-radar-build/ "FMCW Radar")。

首先，[Henrik]使用 CST 软件设计了天线，这是一种专门用于这类工作的电磁模拟程序。他的最终设计包括一个 100 毫米×85 毫米孔径、90 毫米长的喇叭形状。软件模拟显示预期增益为 14.4dB，波束宽度为 35 度。他的旧水壶只有大约 6dB，宽度在 100 度左右。

天线的二维组件都是从金属片上切割下来的。这些零件然后被焊接在一起。[Henrik]承认，在某些情况下，他的精度可能会相差 2mm，这将影响天线的性能。在两个喇叭之间还放置了一片金属，以减少天线之间的耦合。

[Henrik]在当地足球场测试他的新天线。他发现现实生活中的天线表现不如模拟的好。他能够在 44 度的场宽下实现大约 10dB 的增益。这仍然是对 cantenna 设计的巨大改进。

如果你还没有尝试过 Radar，看看[Greg Charvat 的] [鼓励的话语](http://hackaday.com/2014/02/24/guest-post-try-radar-for-your-next-project/)，然后投入进去吧！