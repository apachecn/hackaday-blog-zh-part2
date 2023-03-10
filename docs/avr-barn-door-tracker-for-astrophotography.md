# 用于天体摄影的 AVR 谷仓门跟踪器

> 原文：<https://hackaday.com/2014/01/23/avr-barn-door-tracker-for-astrophotography/>

![zzjBarnDoorTracker](img/4d038e61d3c4a65a563a3fc85d6f8414.png)

【zigzag Joe】首次涉足天体摄影是[这款令人印象深刻的 AVR 谷仓门跟踪器](http://imgur.com/a/PfbjU)，它在不清空银行账户的情况下提升了他的夜空摄影游戏。如果你从未听说过天体摄影，你应该浏览一下[的维基百科页面](http://en.wikipedia.org/wiki/Astrophotography)和/或[的子页面](http://www.reddit.com/r/astrophotography/)。这个想法是通过长时间曝光来捕捉人眼无法察觉的图像。不幸的是，我们都居住的大岩石球有旋转的趋势，这意味着你需要移动相机来保持夜空的框架。

大多数追踪器需要精密的部件和制造，这超出了 ZigZagJoe 的能力范围。相反，他用[cloud bait Observatory model](http://www.cloudbait.com/projects/barndoor.html)找到了一个解决方案，据我们所知，它看起来有点类似于我们去年推出的追踪器。与去年使用 ATmega32u4 分线板不同的是,[ZigZagJoe 的]追踪器使用 ATTiny85 作为大脑，运行预先配置的表格来确定步频与时间的关系。

你可能会问“照片在哪里？”看起来[ZigZagJoe]最近一直被云所困扰，但他承诺它们即将到来。前往 reddit 上的[他的构建线程，了解关于该项目的设计的更多细节，并希望未来发布一些图片。并且通过](http://www.reddit.com/r/astrophotography/comments/1vx4vy/yet_another_barn_door_tracker_build_album/)[这个站点](http://ridetheclown.com/downloads/BarnTracker/)获得一堆关于构建你自己的文件。