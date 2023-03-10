# 说话，脚踏控制的虚拟 Bench 台式探头

> 原文：<https://hackaday.com/2015/07/29/talking-foot-pedal-controlled-bench-probes-for-virtualbench/>

在调试和测试阶段，开发新产品可能具有挑战性，通常你会低着头试图探测某个 SOT23 晶体管的引线，当你拿到引线时，你会抬起眼睛，发现万用表测量的是电阻而不是电压。

[Charles]在他的 NI 虚拟仪器上增加了这个问题。它有一个完全由 PC 驱动的界面，这个界面可能在一个方便鼠标移动的位置，也可能不在。幸运的是，倪刚刚发布了一个用于 5 合 1 实验室测试站的 API，[查尔斯]很快就完成了一个 python 包装器，这使他能够最终控制仪器。

将脚本绑在 USB 踏板上，并使用谷歌的 API 添加一些文本到语音的功能[Charles]可以轻松地从连续性切换到电压到电阻和任何他喜欢的东西，只需轻轻一脚，听着测量结果，确保他的眼睛永远不会离开有短路风险的工作。

休息之后，请加入我们，观看一段简短的视频演示。

[https://www.youtube.com/embed/1NOQRLI39es?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/1NOQRLI39es?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)