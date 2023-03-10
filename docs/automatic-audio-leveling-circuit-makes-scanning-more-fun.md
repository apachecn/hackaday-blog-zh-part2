# 自动音频调平电路使扫描更有趣

> 原文：<https://hackaday.com/2014/06/29/automatic-audio-leveling-circuit-makes-scanning-more-fun/>

![alan-scope1](img/89eeb7496e8a3d0676ef2daf184bf136.png)

[艾伦的]朋友带着一个问题来找他。他喜欢听他的扫描仪，但讨厌电台之间的音量差异。一些发射机的音量很小，其他的几乎会把他的扬声器吹爆。为了解决这个问题，[艾伦]用他在实验室里找到的零件搭建了一个快速自动调平电路(YouTube 链接)。

[Alan]c![alan-scope2](img/5592b9d733133ca95bfac43c0f71fcfe.png)电路并不新鲜，他在视频中指出，各种音频限制、压缩和自动增益控制电路已经在互联网上流传多年。他带来的是他解释电路操作的一贯天赋，用示波器给出了大量的例子。(对于那些不知道的人，当[Alan]不是为了好玩而构建电路时，他是 Tektronix 的一名 RF 应用工程师)。

艾伦的电路本质上是一个衰减器。它接收扬声器级别的音频(完全是桌面扫描仪中的音频)，并输出峰峰值约为 50mv 的有限信号，足以驱动一个辅助放大器。衰减器由一个电阻和一对 1N34A 锗二极管组成。施加到二极管上的偏置电流越多，它们对主音频信号的衰减就越大。二极管偏置电流由主音频信号驱动的基于晶体管的峰值检测器电路产生。但是不要只相信我们的话，休息后再看视频。

[https://www.youtube.com/embed/1h0FZJYXQ_w?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/1h0FZJYXQ_w?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)