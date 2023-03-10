# 认真对待业余无线电；从头开始设计和构建单边带收发器第 1 部分

> 原文：<https://hackaday.com/2015/02/02/get-serious-with-amateur-radio-design-build-a-single-sideband-transceiver-from-scratch-part-1/>

业余无线电是唯一的爱好，为其许可的运营商提供了合法设计、建造和操作连接到无限天线阵列的高功率无线电收发器的机会，以便在世界任何地方进行通信。这种通信系统最复杂的部分是单边带(SSB)高频(HF)收发器。事实上，由于低成本业余设备的激增，只有极少数顽固分子实际设计、从头开始构建并操作自己的单边带收发器。我就是其中一个顽固分子，在这篇文章中，我将告诉你如何开始。

## 无线电架构

为了理解单边带收发器的工作原理，我们必须先回顾一下无线电接收器的基本架构。我最喜欢抽象无线电架构的方式是考虑框图层面的一切:滤波器、放大器、乘法器(我们称之为混频器)，并假设所有模块都是阻抗匹配的。

最早的无线电架构被称为调谐射频(TRF)，它在 20 世纪 20 年代中期到后期被广泛应用于消费类接收机。信号链由一个天线组成，用于收集无线电信号，该信号馈入四级滤波，中间穿插三级放大。最后一个可调滤波器的输出馈入包络检波器(一个二极管)，解调后的音频在检波器中被放大并从扬声器中播放出来。要调谐一个电台，你只需将每个滤波器调谐到所需的频率。后来的型号将每个滤波器部分的可变电容器机械耦合在一起，这样用户只需转动一个旋钮就可以调谐到一个电台。

 [![TRF_radio_example](img/c59562cb9e4ff39541d3f7c315609ebd.png "TRF_radio_example")](https://hackaday.com/2015/02/02/get-serious-with-amateur-radio-design-build-a-single-sideband-transceiver-from-scratch-part-1/trf_radio_example-2/)  [![TRF_radio_CBK20B_example](img/c4083a50c5c47c3262ea0fe3aa93d4c4.png "TRF_radio_CBK20B_example")](https://hackaday.com/2015/02/02/get-serious-with-amateur-radio-design-build-a-single-sideband-transceiver-from-scratch-part-1/trf_radio_cbk20b_example-2/)  [![CBK_20B_outside](img/218faabe8b6eeed1cf573ae106422583.png "CBK_20B_outside")](https://hackaday.com/2015/02/02/get-serious-with-amateur-radio-design-build-a-single-sideband-transceiver-from-scratch-part-1/cbk_20b_outside-2/)  [![Block diagram, schematic, and, photos of a typical TRF radio.](img/1433f4aaba0e82198e5009f187785f4d.png "CBK_20B_inside")](https://hackaday.com/2015/02/02/get-serious-with-amateur-radio-design-build-a-single-sideband-transceiver-from-scratch-part-1/cbk_20b_inside/) Block diagram, schematic, and, photos of a typical TRF radio.

TRF 架构的问题是多级调谐滤波器价格昂贵。为了解决这个问题，埃德温·阿姆斯特朗(Edwin Armstrong)结合使用了低成本的非调谐滤波器和倍频技术，创造出了超外差架构。

埃德温·阿姆斯特朗意识到了倍频的价值。当两个正弦波形(一个在 frf，另一个在 flo)相乘时，结果是这两个频率的和与差:F _ if = F _ RF–F _ lo 和 F_if = F_rf + F_lo。

[![How a frequency mixer works.](img/5348e242532eccc9602e4d61ab3742e2.png)](https://hackaday.com/wp-content/uploads/2015/01/mixer_basics.png)

How a frequency mixer works.

在 RF 设计中，我们将乘法器称为[混频器](http://en.wikipedia.org/wiki/Frequency_mixer)。在超外差接收机中，通过使用混频器和可变频率振荡器(VFO 或本地振荡器),期望的 RF 信号被下变频到中频(IF ),其中存在多级滤波器以选择信号传递到包络检波器。换句话说，混频器的两个乘积之一必须等于 IF 滤波器的中心频率。要改变收音机的接收频率，你所要做的就是改变 VFO 的频率。

下图显示了 40 年代后期的台式 am 收音机的框图，其中收音机以频率 FRF = OS C1–455 kHz 的频率调谐电台。改变 OSC1 的频率会改变收音机调谐到 frf 的频率。

 [![Block diagram, schematic, and photos of a typical superheterodyne broadcast band receiver.](img/de2ab133b0a90131cccbce352da59f8e.png "basic_AM_heterodyne_radio")](https://hackaday.com/2015/02/02/get-serious-with-amateur-radio-design-build-a-single-sideband-transceiver-from-scratch-part-1/basic_am_heterodyne_radio-2/) Block diagram, schematic, and photos of a typical superheterodyne broadcast band receiver. [![olympic_6606_schematic_callouts](img/59121e653a62bcc9e4251d010472d421.png "olympic_6606_schematic_callouts")](https://hackaday.com/2015/02/02/get-serious-with-amateur-radio-design-build-a-single-sideband-transceiver-from-scratch-part-1/olympic_6606_schematic_callouts-2/)  [![olympic_6606_front](img/8d58a5761b71ada149c5c2c82bc2f2a2.png "olympic_6606_front")](https://hackaday.com/2015/02/02/get-serious-with-amateur-radio-design-build-a-single-sideband-transceiver-from-scratch-part-1/olympic_6606_front-2/)  [![olympic_6606_inside](img/b1a62d8e993a597f33a47be0fd169b0d.png "olympic_6606_inside")](https://hackaday.com/2015/02/02/get-serious-with-amateur-radio-design-build-a-single-sideband-transceiver-from-scratch-part-1/olympic_6606_inside/) 

## 单边带接收机

SSB 接收机不再使用包络检波器解调无线电信号，而是使用第二个混频器将 IF 再次下变频至音频范围(该第二个混频器有时称为积检波器)。结果被放大并通过扬声器输出。

单边带接收机听到的实际上是无线电频谱乘以音频频谱，所以我们可以听到它。你听到的是真实的无线电波。

在这种情况下，IF 滤波器的带宽在 1.8 到 2.5 kHz 之间，与人类语音的带宽相匹配。IF 滤波器的中心频率和第二个本振决定选择什么边带，是上边带(USB)还是下边带(LSB)。USB 和 LSB 指的是将人的声音分别转换到载波频率之上和之下。

 [![Blog diagram of a 20m SSB receiver and representative plots of the signals at each stage within the receiver.](img/8b972ce49546925a4e74193e8a3f5b92.png "SSB_front_end")](https://hackaday.com/2015/02/02/get-serious-with-amateur-radio-design-build-a-single-sideband-transceiver-from-scratch-part-1/ssb_front_end/) Blog diagram of a 20m SSB receiver and representative plots of the signals at each stage within the receiver. [![SSB_IF_and_product_det](img/87adb2346e9e64ab11b9f14bf70a4470.png "SSB_IF_and_product_det")](https://hackaday.com/2015/02/02/get-serious-with-amateur-radio-design-build-a-single-sideband-transceiver-from-scratch-part-1/ssb_if_and_product_det/)  [![SSB_reciever_block_diagram](img/3c78a933b5671b2d393e440926e488c6.png "SSB_reciever_block_diagram")](https://hackaday.com/2015/02/02/get-serious-with-amateur-radio-design-build-a-single-sideband-transceiver-from-scratch-part-1/ssb_reciever_block_diagram/) 

## 单边带发射机

单边带发射机就是单边带接收机的反例。滤波器和现代双平衡混频器双向工作。放大器以这种方式连接到继电器或引脚 didoes，因此它们可以在发射模式下反转。当你发射单边带时，你的声音被上变频到无线电频谱，放大，然后从天线发射出去。

[![Block diagram of a 20m SSB transmitter.](img/81860ee7904fdba870d2d7e1f9852843.png)](https://hackaday.com/wp-content/uploads/2015/01/ssb_transmit_block_diagram.png)

Block diagram of a 20m SSB transmitter.

## 20m 单边带收发器

我开发的第一个单边带收发器是为 20m 设计的，这可以说是最好玩的 HF 频段。海事网在 14.300。白天有很多 DX。在康涅狄格州的海岸线上，我可以用 40 瓦和一个半波偶极天线例行公事地在西欧和俄罗斯腹地工作。

 [![A 20m SSB transceiver built from scratch.](img/b005c856e90adaf35a570903bff0d03d.png "homebrew_20m_SSB_radio")](https://hackaday.com/2015/02/02/get-serious-with-amateur-radio-design-build-a-single-sideband-transceiver-from-scratch-part-1/homebrew_20m_ssb_radio/) A 20m SSB transceiver built from scratch. [![HPIM2026](img/de823b90a6f9b8aea05e60d4e1151046.png "HPIM2026")](https://hackaday.com/2015/02/02/get-serious-with-amateur-radio-design-build-a-single-sideband-transceiver-from-scratch-part-1/hpim2026/)  [![HPIM2116](img/01957bc081ad1a2d55eafffb6292fab0.png "HPIM2116")](https://hackaday.com/2015/02/02/get-serious-with-amateur-radio-design-build-a-single-sideband-transceiver-from-scratch-part-1/hpim2116/)  [![HPIM2222](img/d3654f99759ad640619c125462e2adb2.png "HPIM2222")](https://hackaday.com/2015/02/02/get-serious-with-amateur-radio-design-build-a-single-sideband-transceiver-from-scratch-part-1/hpim2222/) 

该收发器的框图如上所示。许多细节、图表和附加信息可以在[这里](http://glcharvat.com/Dr._Gregory_L._Charvat_Projects/Home_Brew_20M_SSB_Transciever.html)找到。这款无线电代表了绝大多数单边带收发器架构。

## 后续步骤

我已经将无线电电路抽象为框图级别。一旦理解了模块，就可以在高层次上进行设计。框图准备好后，可以选择电路、IC 或模块来填充框图。有些电路是从书上借来的，或者是从书上的某个设计中改编的。50 欧姆集成电路和模块的一个重要来源是[微型电路](http://www.minicircuits.com/homepage/homepage.html)。其他应用需要合成定制的梯形网络，RF 前端滤波器就是这种情况。这些是寻找、借用或综合这些电路或整个无线电架构的绝佳资源，甚至:

[ARRL 手册](http://www.arrl.org/arrl-handbook-2015)
[面向无线电爱好者的固态设计](http://www.amazon.com/Solid-State-Design-Radio-Amateur/dp/0872590402)
[约瑟夫·卡尔的射频电路设计秘密](http://www.amazon.com/Secrets-Circuit-Design-Joseph-Carr/dp/0071370676/ref=sr_1_1?s=books&ie=UTF8&qid=1422149314&sr=1-1&keywords=secrets+of+RF+circuit+design)
[克里斯·博维克射频电路设计](http://www.amazon.com/RF-Circuit-Design-Christopher-Bowick/dp/0750699469/ref=sr_1_2?s=books&ie=UTF8&qid=1422149353&sr=1-2&keywords=RF+Circuit+Design+Chris+Bowick)
[罗德的通信接收机](http://www.amazon.com/Communications-Receivers-Software-Radios-Design/dp/0071361219/ref=asap_bc?ie=UTF8)
[QST 杂志](http://www.arrl.org/qst)
[QEX 杂志](http://www.arrl.org/qex)

* * *

## 构建它:

基础 RF 设计还有更多的内容，真正学习的唯一方法就是开始做。尽可能多的向别人借电路。拼凑你的收音机。你会在设计的每个方面做得更好。跳进来吧！没有什么比在自己制作的收发器上进行长途联系更令人满意的了。我期待着尽快与你们中的一些人在广播中交流！

## 确认

我的表妹，[朱丽叶·赫尔利](http://www.everchangellc.com/owner-bio)，MBA，MSF，MAC，负责编辑这篇文章。

* * *

## 作者简介

[Gregory L. Charvat](http://glcharvat.com/Dr._Gregory_L._Charvat_Projects/About.html) 只操作他白手起家建造的无线电设备，是[小型短程雷达系统](http://www.crcpress.com/product/isbn/9781439865996)的作者， [Hyperfine Research Inc.](http://www.hyperfine-research.com) 、 [Butterfly Network Inc.](http://www.technologyreview.com/news/532166/with-100-million-entrepreneur-sees-path-to-disrupt-medical-imaging/) (这两家公司都是 [4catalyzer](http://www.4catalyzer.com) 公司)的联合创始人，麻省理工学院媒体实验室 Camera Culture Group 的客座研究科学家， [Gregory L. Charvat 关于电气工程实用方法的系列文章的编辑，](http://glcharvat.com/Dr._Gregory_L._Charvat_Projects/Book_Series_on_Electrical_Engineering.html)的客座评论员他是麻省理工学院林肯实验室的技术人员，他在穿墙雷达方面的工作赢得了 2010 年 MSS 三军雷达研讨会的最佳论文，并且是 2011 年 Provost 研究亮点的麻省理工学院办公室。他曾在麻省理工学院教授短期雷达课程，他的“构建小型雷达”课程是 2011 年排名第一的麻省理工学院专业教育课程，并被其他大学、实验室和私人组织广泛采用。从早年开始，Greg 开发了许多雷达系统、铁路 SAR 成像传感器、相控阵雷达系统；拥有多项专利；并开发了许多其他传感器、无线电和音频设备。他撰写了许多出版物，并因其作品受到媒体的关注。Greg 于 2007 年获得密歇根州立大学电气工程博士学位，2003 年获得 MSEE，2002 年获得 BSEE，他是 IEEE 的资深会员，在 2010 年、2013 年和 2016 年 IEEE 国际相控阵系统和技术研讨会指导委员会任职，并于 2010 年至 2011 年担任 IEEE AP-S Boston 分会主席