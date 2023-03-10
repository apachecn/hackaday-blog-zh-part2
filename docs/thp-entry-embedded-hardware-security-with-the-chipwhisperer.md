# THP 参赛作品:使用 ChipWhisperer 实现嵌入式硬件安全

> 原文：<https://hackaday.com/2014/07/04/thp-entry-embedded-hardware-security-with-the-chipwhisperer/>

![KONICA MINOLTA DIGITAL CAMERA](img/19f54c12e579bb07f9db4ec0666c590f.png)

有成千上万的论文讨论嵌入式硬件安全的各个方面，还有几十本书涉及同一主题。文献中讨论的攻击非常酷——像侧信道功耗分析和用于从系统中提取密钥的时钟毛刺。这些论文中的实验装置非常昂贵——你可以花更少的钱买一辆新车。[coflynn]对这些工具的价格感到沮丧，[并认为建造自己的](http://hackaday.io/project/956-ChipWhisperer)将有助于获得 Hackaday 奖。

ChipWhisperer 的硬件部分包括一个分线板，带有一个 FPGA、ADC 和用于许多不同探针的连接器、适配器、分线板和一个目标板，有了所有这些工具，说[coflynn]可以对一批*嵌入式硬件进行功耗分析攻击并不为过。*

开源硬件只是这个入口的一部分。这个项目最大的焦点是用于分析探针和目标板记录的开源软件。有了这个软件，任何人都可以监控芯片运行加密功能时的功耗，或者为设备中的一些非预期功能干扰时钟。为了与所有关于这些攻击的文献的学术谱系保持一致，[对于那些崭露头角的安全研究人员来说,](http://newae.com/sidechannel/cwdocs/)有大量关于芯片密语的教程。非常酷的东西，可以说是 Hackaday 奖最具技术性的作品之一。

下面视频。

* * *

![SpaceWrencher](img/4892437613088ab3882681a2ec04a2bb.png) **本帖介绍的项目是[黑客大奖](http://hackaday.io/prize)中的一个参赛项目。建造一些令人敬畏的东西，赢得太空之旅或数百个其他奖品。**

[https://www.youtube.com/embed/Ya7UsmJTpd8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&hd=1&wmode=transparent](https://www.youtube.com/embed/Ya7UsmJTpd8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&hd=1&wmode=transparent)