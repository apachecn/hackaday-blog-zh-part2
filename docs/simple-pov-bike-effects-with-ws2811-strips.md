# 带 WS2811 条的简单 POV 自行车效果

> 原文：<https://hackaday.com/2014/10/27/simple-pov-bike-effects-with-ws2811-strips/>

[Andrew]和[一起写了一篇关于视觉自行车辐条黑客](http://www.instructables.com/id/Bike-wheel-WS2811-LED-effects-with-Arduino/)的经典持久性的新文章。虽然许多 POV 设置使用[定制 PCB](http://hackaday.com/2012/08/06/pov-bike-wheels-with-the-msp430/)和分立 LED，但【Andrew】的设计使用现成的组件:WS2811 LED 灯条、Arduino、Invensense IMU 分线板和一些小型 LiPo 电池。

[Andrew]还实现了一种控制灯光的巧妙方法。他的代码检测到骑车人何时按特定模式踩刹车，这允许在不同的灯模式之间切换。他确实注意到，由于他的 IMU 的一些问题，这种方法不太可靠，所以现在他也能感觉到骑车人何时敲击车把。

如果你想建立自己的自行车视点设置，你很幸运。[Andrew]写了详细的说明，概述了整个构建过程。他还提供了每个部分的源代码链接，使构建自己的设置更加容易。他的设计也很实惠，每个轮子不到 50 美元。休息之后，请观看[Andrew]的设置视频。

[https://player.vimeo.com/video/110069992](https://player.vimeo.com/video/110069992)