# 欢迎来到老学校:修复古董收音机

> 原文：<https://hackaday.com/2014/09/09/welcome-to-the-old-school-restoring-antique-radios/>

二战前，无线电是大众传播领域的一场革命，就像今天的互联网一样。财富的创造和失去，帝国的建立，史诗般的专利战接踵而至，所有这一切导致世界比以往任何时候都更加紧密地联系在一起，[这造就了一个真正伟大的故事](http://www.amazon.com/Empire-Air-The-Made-Radio/dp/0060182156/ref=sr_1_2?ie=UTF8&qid=1409881598&sr=8-2&keywords=empire+of+the+air)(以及一部伟大的[本·伯恩斯纪录片](http://www.pbs.org/kenburns/empire/))。

上个月，我们向您展示了如何[改装老式收音机，通过它播放您自己的音频源](http://hackaday.com/2014/08/11/poor-audio-quality-made-great-listen-to-vintage-music-using-an-antique-radio-without-removing-the-insides/)，同时重复使用现有的电子设备并保持其功能。在这篇文章中，我们将向你展示如何修复任何真空管收音机。你将从一个不同的时代学习基本的修理/修复程序，那个时代实际上值得修理消费电子产品。深入历史，了解 20 世纪上半叶最具影响力的技术！

在早期，收音机是非常昂贵的消费设备，在某些情况下，其价格相当于或超过一辆汽车或一栋房子。出于这个原因，许多听众求助于建立自己的。 [Edwin Armstrong](http://users.erols.com/oldradio/) 开发了[外差式接收机](http://en.wikipedia.org/wiki/Superheterodyne_receiver)，该接收机使用倍频将所需信号下移到中频，在中频进行滤波和检测，从而降低了成本并增加了无线电技术的使用。外差式接收机的成本远低于以前被称为[调谐射频](http://en.wikipedia.org/wiki/Tuned_radio_frequency_receiver) (TRF)的架构，以前的无线电只是一个非常大的可调谐带通滤波器(通常有 3 或 4 个部分)，每个部分之间都有放大器，必须在整个 AM 广播波段进行调谐。TRF 架构非常昂贵，因为在一个完整倍频程内维持一个窄的 10 KHz 带通滤波器极具挑战性，并且比仅使用一个固定滤波器需要更高的精度，而固定滤波器可以大规模生产并且处于较低的频率。

 [![TRF_radio_example](img/8f081900d49d92545f1844d48762ee0a.png "TRF_radio_example")](https://hackaday.com/2014/09/09/welcome-to-the-old-school-restoring-antique-radios/trf_radio_example/)  [![Example of a TRF radio architecture used in the mid-to-late 1920's.](img/6a67af3afa03d40421d0f1ec6025c220.png "TRF_radio_CBK20B_example")](https://hackaday.com/2014/09/09/welcome-to-the-old-school-restoring-antique-radios/trf_radio_cbk20b_example/) Example of a TRF radio architecture used in the mid-to-late 1920’s. [![CBK_20B_outside](img/893d218a86376bab9b40bb126f15da0a.png "CBK_20B_outside")](https://hackaday.com/2014/09/09/welcome-to-the-old-school-restoring-antique-radios/cbk_20b_outside/)  [![The Heterodyne architecture developed by Edwin Armstrong revolutionized radio, reducing costs, improving performance, and democratizing access to this technology thereby revolutionizing the way humankind communicates on a massive scale.](img/753ae21295dce4267387d414a556d0ea.png "basic_AM_heterodyne_radio")](https://hackaday.com/2014/09/09/welcome-to-the-old-school-restoring-antique-radios/basic_am_heterodyne_radio/) The Heterodyne architecture developed by Edwin Armstrong revolutionized radio, reducing costs, improving performance, and democratizing access to this technology thereby revolutionizing the way humankind communicates on a massive scale. [![olympic_6606_schematic_callouts](img/f588613058bda73e6d9bbb5afba87c4e.png "olympic_6606_schematic_callouts")](https://hackaday.com/2014/09/09/welcome-to-the-old-school-restoring-antique-radios/olympic_6606_schematic_callouts/)  [![olympic_6606_front](img/772fbb589ee03599b273b7d06e920554.png "olympic_6606_front")](https://hackaday.com/2014/09/09/welcome-to-the-old-school-restoring-antique-radios/olympic_6606_front/) 

#### **危险，危险，高压！**

使用旧的无线电设备时要非常小心。是的，这些收音机内部有很高的电压。许多人甚至将线路的热端直接连接到他们的金属底盘(称为热底盘收音机)，特别是大多数战后的台式收音机。

#### **操作指南**

古董收音机可以是功能性的产品，显示你对旧款式的欣赏和修理任何东西的能力。这种爱好是任何有基本电子技能的人都能达到的。按照以下一般步骤恢复您的无线电:

1.  不要打开你的收音机。如果在更换电容器之前接通电源，可能会造成损坏。电容器有几种类型，但通常会随时间而衰减的是电解电容器(通常出现在电源和音频输出电路中)和蜡纸耦合电容器。
2.  找一本维修手册。大多数都可以在网上找到。
3.  将所有电解电容器和纸电容器更换为具有相似值、相同或更好额定电压的新电容器。
4.  仔细检查并更换任何看起来损坏的部件，例如烧毁的电阻器。
5.  使用[调光灯泡测试仪](http://www.antiqueradio.org/dimbulb.htm)测试收音机，调光灯泡测试仪是一个 60 到 100 瓦的灯泡，与收音机的线电压串联。如果过一会儿灯泡变暗，那么收音机内的 B+线可能没有短路。你甚至可能听到噼啪声或一些信号传来。
6.  如果它通过了调光灯泡测试，然后尝试直接离线给它通电。大多数老式收音机在更换电容器后仍能工作。
7.  如果不起作用，则通过在 If 或 RF 注入信号，替换电阻或偶尔替换需要的电子管，在电路中跟踪信号。旧电阻器有随时间而增值的趋势。通常电子管收音机的坏级是由于电阻的阻值增加到了使电子管截止的程度。电子管通常不是导致收音机停止使用的原因。发现不良电阻的最快方法是探测管针电压。给定特定的伏特表阻抗，在你的收音机的维修手册中会有一个管针电压图表。只要发现电压超出容差(大于 10%)，就检查连接到该引脚的电阻或连接到该引脚的其他电路。
8.  如果站太弱，则按照维修手册中的程序进行校准。
9.  打开收音机。应该能行！

从这个视频开始的视频系列很好地涵盖了这些基础知识:

[https://www.youtube.com/embed/WylSXLou9y0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/WylSXLou9y0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

#### RCA Radiola 18

这是 20 世纪 20 年代末 TRF 接收器修复的一个很好的例子。更换了电源电容器和少量纸耦合电容器。灰尘和污垢被清除掉了。木质围栏被清理干净并打了蜡。对于许多像这样的 TRF 接收器来说，对准是不需要的。对于一个非常灵敏的接收机来说，性能出奇的好。

 [![DSC_0133](img/9d23fdfbb05f39c914a4aedb6a0732a7.png "DSC_0133")](https://hackaday.com/2014/09/09/welcome-to-the-old-school-restoring-antique-radios/dsc_0133/)  [![DSC_0120](img/5be3166490bea9fc72573b771130abca.png "DSC_0120")](https://hackaday.com/2014/09/09/welcome-to-the-old-school-restoring-antique-radios/dsc_0120-2/)  [![Example of a late-1920's TRF receiver, the RCA Radiola 18.](img/a03693ebc2cebe82d6c8a374ea46ff7d.png "DSC_0078")](https://hackaday.com/2014/09/09/welcome-to-the-old-school-restoring-antique-radios/dsc_0078/) Example of a late-1920’s TRF receiver, the RCA Radiola 18\.

[https://www.youtube.com/embed/NcKsgI_9I70?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/NcKsgI_9I70?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

#### **银石型号 4686**

这是一个标志性的美国控制台收音机的例子。这台收音机制造于 1937 年，见证了许多历史:大萧条、第二次世界大战，很可能还有朝鲜战争，直到它退役。这一代无线电首次利用了外差接收机架构。由于这个原因，这些收音机在很大的频率范围内调谐。他们不仅可以调谐标准的调幅广播波段，还可以覆盖 2-18 兆赫的短波频率。修复这些收音机并不困难。赚了几百万。在跳蚤市场和广播节目中购买它们并不贵。如果你找不到合适的零件，再买一个并回收。

 [![HPIM2857](img/8a4ebf4c5045d4a816cca3415ee2d06f.png "HPIM2857")](https://hackaday.com/2014/09/09/welcome-to-the-old-school-restoring-antique-radios/hpim2857/)  [![The iconic American console radio.](img/85666117a73d0db2ca83bc0b11667e45.png "HPIM2844")](https://hackaday.com/2014/09/09/welcome-to-the-old-school-restoring-antique-radios/hpim2844/) The iconic American console radio. [![HPIM2859](img/966c9efdd4f7981537e9c83e05e7a11c.png "HPIM2859")](https://hackaday.com/2014/09/09/welcome-to-the-old-school-restoring-antique-radios/hpim2859/) 

[https://www.youtube.com/embed/SkF-H6EB-yg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/SkF-H6EB-yg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

#### **真力时 K725**

到 20 世纪 50 年代，收音机随处可见。调频广播以其高保真度开始流行起来。桌面收音机，如[这台](http://glcharvat.com/Dr._Gregory_L._Charvat_Projects/Restoration_of_a_Zenith_K725.html)在一个紧凑的包装中提供了 AM 和 FM 广播波段，具有 20 世纪 50 年代的风格，很像汽车、喷气式飞机、火箭、尾翼和铬合金，以及当时其他令人兴奋的技术。这款收音机在音频输出中特别使用了负反馈，提供了蓬勃发展的高保真音频。不幸的是，这是一个热底盘收音机，电源线直接连接到内部的金属底盘，因此在维修时必须使用一个[隔离变压器](http://en.wikipedia.org/wiki/Isolation_transformer)与电源线串联。

 [![HPIM1683](img/5a36930b01134b83482d07382255be50.png "HPIM1683")](https://hackaday.com/2014/09/09/welcome-to-the-old-school-restoring-antique-radios/hpim1683/)  [![HPIM1682](img/72848adacb07a1a85942bed38d60ffd3.png "HPIM1682")](https://hackaday.com/2014/09/09/welcome-to-the-old-school-restoring-antique-radios/hpim1682/)  [![The ubiquitous AM/FM table top radio of the 1950's.](img/545f087a46f8ded24b3528d3e61ff201.png "HPIM1680")](https://hackaday.com/2014/09/09/welcome-to-the-old-school-restoring-antique-radios/hpim1680/) The ubiquitous AM/FM table top radio of the 1950’s.

#### **通过修复了解历史**

是时候去跳蚤市场买几台旧收音机了！自学修理老式电子产品的技能，接触过去。学习独特的故障排除技能，这将提升您的日常职业生涯。不管是电子管还是晶体管，一个经验丰富的工程师能够运用今天和昨天的技术。

#### **参考文献**

*   加入古董无线协会，阅读关于无线技术历史的双月刊。
*   从[论坛获得帮助:www.antiquradios.com](http://www.antiqueradios.com/forums/index.php)
*   [bandersontv 的 youtube 频道](https://www.youtube.com/user/bandersentv)。

#### **确认**

我的表妹，[朱丽叶·赫尔利](http://www.everchangellc.com/owner-bio)，MBA，MSF，MAC，负责编辑这篇文章。

#### **作者简介:**

[Gregory L. Charvat](http://glcharvat.com/Dr._Gregory_L._Charvat_Projects/About.html) 是《小型和短程雷达系统[的作者](http://www.amazon.com/Short-Range-Practical-Approaches-Electrical-Engineering/dp/143986599X)，Camera Culture Group 麻省理工学院媒体实验室的客座研究科学家，Hyperfine Research Inc .、Butterfly Network Inc .的联合创始人，Gregory L. Charvat 电气工程实用方法系列的编辑，以及 CNN、CBS、Sky News 等的客座评论员。他是麻省理工学院林肯实验室的一名技术人员，他在穿墙雷达方面的工作赢得了 2010 年 MSS 三军雷达研讨会的最佳论文，并且是 2011 年 Provost 研究亮点的麻省理工学院办公室。他曾在麻省理工学院教授短期雷达课程，他的“构建小型雷达”课程是 2011 年排名第一的麻省理工学院专业教育课程，并被其他大学、实验室和私人组织广泛采用。从早年开始，Greg 开发了许多雷达系统、铁路 SAR 成像传感器、相控阵雷达系统；拥有多项专利；并开发了许多其他传感器、无线电和音频设备。他撰写了许多出版物，并因其作品受到媒体的关注。Greg 于 2007 年获得密歇根州立大学电气工程博士学位，2003 年获得 MSEE 博士学位，2002 年获得 BSEE 博士学位，他是 IEEE 的高级成员，曾在 2010 年、2013 年和 2016 年 IEEE 国际相控阵系统和技术研讨会的指导委员会任职，并于 2010 年至 2011 年担任 IEEE AP-S Boston 分会主席。