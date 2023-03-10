# 糟糕的音质成就了伟大:用古董收音机听古典音乐，不用拆下内部

> 原文：<https://hackaday.com/2014/08/11/poor-audio-quality-made-great-listen-to-vintage-music-using-an-antique-radio-without-removing-the-insides/>

 [![trans_radio4](img/bee8356b5f1f70284de07c394c88652f.png "trans_radio4")](https://hackaday.com/2014/08/11/poor-audio-quality-made-great-listen-to-vintage-music-using-an-antique-radio-without-removing-the-insides/trans_radio4/)  [![fig_1_cbk20b_w_ipod](img/1f5e91ae55a89354ed80ee1931fd3103.png "fig_1_cbk20b_w_ipod")](https://hackaday.com/2014/08/11/poor-audio-quality-made-great-listen-to-vintage-music-using-an-antique-radio-without-removing-the-insides/fig_1_cbk20b_w_ipod/)  [![fig_4_olympic_6_606](img/881135563f0b49fa3075018716f7febb.png "fig_4_olympic_6_606")](https://hackaday.com/2014/08/11/poor-audio-quality-made-great-listen-to-vintage-music-using-an-antique-radio-without-removing-the-insides/fig_4_olympic_6_606/) 

有时候不是你的设备重现声音有多好，而是有多差。在之前的一篇黑客帖子中，老式晶体管收音机的电路被移除，以便安装蓝牙音频源并连接到扬声器。相比之下，这篇文章将展示如何使用老式收音机的现有电路来播放您自己的音频源，同时保留收音机的功能。您将能够通过收音机自带的音频信号链播放音乐，然后切换回 AM 模式并收听球赛。发表声明——适应并使用老式电子产品。

1950 年前的录音在高保真系统上播放时听起来很嘈杂，但通过战前的控制台收音机播放时就不会了。一首古老的宾·克罗斯比曲调听起来像是他用洪亮的调幅声音直接向你的起居室广播。你听不到高频率的“砰”声和“嘶嘶声”,而高保真设备在播放老式录音时会产生这种声音。这可能是由于古董收音机的音频信号链和扬声器不能再现更高的频率。类似地，萨姆·库克用早期的晶体管收音机演奏起来也很棒。这些录音本来是要在它们被录制的那个时代的收音机上播放的。

### 选择古董收音机

老式收音机可以在车库销售，房地产销售，hamfests，古董店，古董收音机交换会议和易趣上找到。已经生产了数百万台收音机。人们经常把它们送人。由于这个原因，古董收音机相对便宜，而且绝大多数并不罕见或有价值。

一般来说，电子管收音机必须维修，甚至可能不工作。晶体管收音机经常在某种程度上工作。尽量找一个干净的，使用电源变压器或者电池的收音机。

点击休息时间，了解如何将这些收音机恢复到工作状态

使用电子管收音机需要注意的一点:您的收音机必须使用电源变压器或电池。为了您自身的安全，您不能使用“热底盘”收音机。“热机箱”无线电使用非极化电源线，其中一根线直接连接到金属机箱，另一根线连接到为无线电提供 B+的整流器。根据电源线插入插座的方式，金属机箱可能会直接连接到热线电压。大多数战后的桌面电子管收音机是“热底盘”收音机。

### 基本程序

找出电路中包络检波器与第一音频级的联系。这通常是音量电位计上游标引脚右侧的第一个引脚(仰视图，从收音机内部向外部看)。接入一个 3 向拨动开关，在外部音频源和收音机之间进行选择。一些较大的老式收音机有外部音频输入；在这种情况下，只需为外部输入制作一个适配器。

### 晶体管收音机

当我想到晶体管收音机时，我会想到类似艾默生先锋 888 的东西。这台美国制造的收音机建于 1957 年，使用 8 个晶体管，具有推挽式音频输出。前面看起来像是 AMF 保龄球馆的一部分。对于 12 美元，这是一个不错的复古购买。

 [![trans_radio4](img/871794dd7f10e9bc6010266fda855b19.png "trans_radio4")](https://hackaday.com/2014/08/11/poor-audio-quality-made-great-listen-to-vintage-music-using-an-antique-radio-without-removing-the-insides/trans_radio4/)  [![trans_radio3](img/5297d3ae88030d40e32a021dec2ca105.png "trans_radio3")](https://hackaday.com/2014/08/11/poor-audio-quality-made-great-listen-to-vintage-music-using-an-antique-radio-without-removing-the-insides/trans_radio3/)  [![Modify a vintage transistor radio so that your audio can be played through its amplifier & speaker while maintaining its original AM radio functionality.](img/a34cd67d05e92144d654af65d81cd558.png "trans_radio1")](https://hackaday.com/2014/08/11/poor-audio-quality-made-great-listen-to-vintage-music-using-an-antique-radio-without-removing-the-insides/trans_radio1/) Modify a vintage transistor radio so that your audio can be played through its amplifier & speaker while maintaining its original AM radio functionality. [![trans_radio2](img/72cafd0e533092ebecbe44825348940f.png "trans_radio2")](https://hackaday.com/2014/08/11/poor-audio-quality-made-great-listen-to-vintage-music-using-an-antique-radio-without-removing-the-insides/trans_radio2/) 

我没有在这台收音机上安装拨动开关，而是修改了它的耳机插孔，以接收音频输入，而不是输出音频。这些收音机上耳机插孔的巧妙之处在于它有一个内置开关。当有东西插入时，这个开关就会打开。我使用这个功能是通过这个开关将 AM 检波器的低电平音频输出到音量电位计。当您插入您的音频源时，AM 信号被打开，然后您的源被馈送到音量电位计。当你移除你的音源时，它又变回了 AM 收音机。有关详细信息，请参见以下示意图:

[![Rather than drill hole in the radio, use its ear phone jack as both the audio input and switch-over from AM to input mode.](img/0d7e60deaa55b9d51bfbd042e736f0d8.png)](https://hackaday.com/wp-content/uploads/2014/08/fig1a-transistor-radio-audio-hack.png)

Rather than drill hole in the radio, use its ear phone jack as both the audio input and switch-over from AM to input mode.

[https://www.youtube.com/embed/dFEiAfV0CjM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/dFEiAfV0CjM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

### 控制台收音机:

科林·B·肯尼迪 20 B 型是 1929 年制造的早期控制台收音机。它的封面自诩是“收音机的皇室”。它使用调谐射频(TRF)架构，与现代接收机有很大不同。

 [![fig_1_cbk20b_w_ipod](img/c9e082971385fbac5cbac760f2106886.png "fig_1_cbk20b_w_ipod")](https://hackaday.com/2014/08/11/poor-audio-quality-made-great-listen-to-vintage-music-using-an-antique-radio-without-removing-the-insides/fig_1_cbk20b_w_ipod/)  [![fig_2_inside_of_cbk20b](img/88addf1d1907074436e6050c8da31c7a.png "fig_2_inside_of_cbk20b")](https://hackaday.com/2014/08/11/poor-audio-quality-made-great-listen-to-vintage-music-using-an-antique-radio-without-removing-the-insides/fig_2_inside_of_cbk20b/) 

方便的是，这个收音机提供了一个没有 RIAA 补偿的留声机输入。许多控制台收音机都有这个功能。它提供了一个高阻抗连接直接进入收音机的音频放大器，允许连接一个 iPod 或其他音频设备。我把一个现代 RCA 插孔连接到这个唱机输入端。

[![Adding an external audio input to a very old console radio.](img/009a0c588d36adfa9022d4e9cf88bec2.png)](https://hackaday.com/wp-content/uploads/2014/08/fig_3_modified_cbk20b_final.jpg)

Adding an external audio input to a very old console radio.

前面板上有一个开关，可以选择“收音机”或“唱机”通过选择“唱机”，来自收音机背面唱机输入连接的线路电平音频信号被输入到检波器三极管的栅极。该三极管的输出馈入音频前置放大器，然后馈入单端音频功率放大器。我用一个简单的分压混频器电路将左右声道合成一个单声道信号，将我的音频设备连接到唱机输入端。

[https://www.youtube.com/embed/bJCIzdMTsJ8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/bJCIzdMTsJ8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

### 古董收音机'音箱'

老式电子管收音机的声音在家里听起来很棒，但如果你能随身携带，会更有趣。为此，我修复了一台[奥林匹克型号 6-606](http://glcharvat.com/Dr._Gregory_L._Charvat_Projects/Retro_Boom_Box_%28with_Ipod_doc%29.html) 电池供电的电子管收音机，并对其进行了改装，这样任何音频源都可以通过它播放。

 [![fig_4_olympic_6_606](img/b506818b66098853707183324b5f9b24.png "fig_4_olympic_6_606")](https://hackaday.com/2014/08/11/poor-audio-quality-made-great-listen-to-vintage-music-using-an-antique-radio-without-removing-the-insides/fig_4_olympic_6_606/)  [![fig_6_rear_of_olympic_ipod_radio_sw](img/a21ff81d25fbd8c177bacc5d7e1af24b.png "fig_6_rear_of_olympic_ipod_radio_sw")](https://hackaday.com/2014/08/11/poor-audio-quality-made-great-listen-to-vintage-music-using-an-antique-radio-without-removing-the-insides/fig_6_rear_of_olympic_ipod_radio_sw/) 

奥林匹克 6-606 建于 1946 年，使用电池或交流电源。不幸的是，如果这个收音机插上电源，那么它的功能就像一个“热机箱”收音机，使用外部音频源太危险了。出于这个原因，我选择完全靠电池来操作它。

实现音频输入需要使用与左右声道串联的电阻，为音频降压变压器供电。这种变压器类似于老式晶体管收音机中的变压器。这个变压器的输出馈入一个 3 路拨动开关，允许您选择 AM 收音机或音频输入。第一个音频级电子管是 1LH4，既用作包络检波器，又用作三极管音频增益级。音频输入/收音机拨动开关是一个双掷开关。它通过将 IF 从开关一极上的包络检波器断开，并通过在包络检波器和音频变压器之间进行选择，作为馈入开关另一极上的音量电位计的音频源，来中断第一音频级的输入。

[![Schematic of minor modifications to the Olympic 6-606 battery tube radio.](img/b4eb55c41913339231218bc14231f98a.png)](https://hackaday.com/wp-content/uploads/2014/08/fig_5_moded_olympic_6_606_final.jpg)

Schematic of minor modifications to the Olympic 6-606 battery tube radio.

Olympic 6-606 需要两个 B 型和两个 A 型电池，为板提供 90 V 电压，为灯丝提供 9V 电压。不幸的是，你不能在当地的五金店找到这些。出于这个原因，我建立了一个相当于两个 B 型的现代电池组，将 10 个 9V 电池串联起来。我模拟了两个 A 型电池，将 6 节 C 型电池串联起来。所有电池都安装在一片铝片上以提供结构，为了安全起见，每个输出端都采用 0.25 A 的保险丝。

用电池给这台收音机供电并不便宜。给电池组充电要花费 30 多美元。幸运的是，电池组可以持续 15+小时。有了这个老式的“音箱”，你可以将电子管的声音带到任何地方，包括聚会、海滩或航行中。在社交场合，这是一个很好的话题。

[https://www.youtube.com/embed/MTsBR-iUm8s?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/MTsBR-iUm8s?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

### 音质更低，乐趣更多

旧唱片通过收音机播放时声音最佳。让老式收音机再次发挥作用！只需简单的操作，你就可以通过老式收音机的音频电路播放音乐或播客，同时保持收音机的功能。

### 参考

*   bandersontv 的[系列](https://www.youtube.com/watch?v=WylSXLou9y0&list=PLMXw4o38auN18TvYGDr0tWli3nH77pdgr)讲述如何修复老式电子产品
*   古董 Radios.com[论坛。](http://www.antiqueradios.com/forums/index.php)

**鸣谢:**我的表妹[茱丽叶·赫利](http://www.everchangellc.com/owner-bio)，负责编辑这篇文章。

**作者简介**
[Gregory L. Charvat](http://glcharvat.com/Dr._Gregory_L._Charvat_Projects/About.html) 是[小型和短程雷达系统](http://www.crcpress.com/product/isbn/9781439865996)的作者，Camera Culture Group 麻省理工学院媒体实验室的客座研究科学家，Hyperfine Research Inc .和 Butterfly Network Inc .的联合创始人，Gregory L. Charvat 电气工程实用方法系列的编辑，以及 CNN、CBS、Sky News 等的客座评论员。从 2007 年 9 月到 2011 年 11 月，他是麻省理工学院林肯实验室的技术人员，他在穿墙雷达方面的工作赢得了 2010 年 MSS 三军雷达研讨会的最佳论文，并且是 2011 年 Provost 研究亮点的麻省理工学院办公室。他曾在麻省理工学院教授短期雷达课程，他的“构建小型雷达”课程是 2011 年排名第一的麻省理工学院专业教育课程，并被其他大学、实验室和私人组织广泛采用。从早年开始，Greg 开发了许多雷达系统、铁路 SAR 成像传感器、相控阵雷达系统；拥有多项专利；并开发了许多其他传感器、无线电和音频设备。他撰写了许多出版物，并因其作品受到了大量媒体的关注。Greg 于 2007 年获得密歇根州立大学电气工程博士学位，2003 年获得 MSEE 博士学位，2002 年获得 BSEE 博士学位，他是 IEEE 的资深会员，曾在 2010 年、2013 年和 2016 年 IEEE 国际相控阵系统和技术研讨会指导委员会任职，并于 2010 年至 2011 年担任 IEEE AP-S Boston 分会主席。