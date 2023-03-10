# THP 四分之一决赛:3GHz 频谱分析仪

> 原文：<https://hackaday.com/2014/09/16/thp-quarterfinalist-3ghz-spectrum-analyzer/>

无线电似乎是 Hackaday 奖的一个非官方主题，一些用于微控制器和软件定义无线电的无线框架进入了四分之一决赛。[roelh]的项目与大多数其他的电台版本有些不同。这是一个简单的频谱分析仪，但工作频率高达 3GHz。

硬件由多个芯片组成，包括 ADL5519 功率检波器、用于本振的 Si4012 和 MAX2680 混频器。Atmel XMega 负责所有的板上处理，在小型 LCD 上显示光谱，将数据写入 SD 卡，并通过 3.5 毫米插孔发送数据，该插孔兼作模拟输入或半双工 RS232 端口。

在下面的视频中可以看到，[roelh]的频谱分析仪差不多完成了，配有一个漂亮的外壳。现在[roelh]正在做文档，将他的源代码移植到英文，并准备好所有的文件供我们真正的评委评判。

* * *

![SpaceWrencher](img/4892437613088ab3882681a2ec04a2bb.png) **本帖介绍的项目是[黑客日奖的四分之一决赛。](http://hackaday.io/list/2864-The-Hackaday-Prize%3A-Semifinalists)**

[https://www.youtube.com/embed/nwh_d2H407A?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/nwh_d2H407A?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)