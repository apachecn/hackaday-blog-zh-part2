# 解决 Arduino 的 Stk500_getsync()错误

> 原文：<https://hackaday.com/2014/11/22/solving-arduinos-stk500_getsync-error/>

[psgarcha]带着一岁大的 Arduino Uno 去国际旅行，回来后发现有些不对劲。每次他试图上传时，都会得到可怕的 avrdude 错误，“stk500_getsync():不同步 resp=0x00”。在尝试上传的过程中，Rx 灯会闪烁几次，但 tx 灯不会。不知何故,“杜伊诺”号出了严重的问题，于是[psgarcha] [深挖以找出原因](http://redhotengineer.blogspot.in/2014/11/my-fight-with-avrdude-stk500getsync-not.html)。

为了测试 Arduino 串行连接的质量，[psgarcha]执行了一个环回测试；基本上是一根插入 Arduino 的 Tx 和 Rx 引脚的电线。通过串行端口发送一条短消息显示，问题不在 USB 电缆、duino 上的 ATmega16u2 或板上的任何痕迹。这需要更多的思考。

错误的主要原因可能是计算机和 duino 之间没有通信，选择了错误的 COM 端口，在 Arduino 文本编辑器中选择了错误的板，或者是时间错误或损坏的引导加载程序。前三个错误现在已经不存在了，只剩下计时错误和损坏的引导程序。然后故障排除转移到订购一个新的程序员，但这仍然不能解决 Uno 的问题。

在成为一名阿杜伊诺修补匠的最大失败之一后，沮丧的[psgarcha]仔细审视了 Uno 董事会。他瞥了一眼 Arduino 巨型板。有些东西看起来不一样了。在 Uno 上，共鸣器爆炸了。至少发现了问题。

用一个可笑的大罐晶体振荡器代替了吹制的部分，[psgarcha]又开始营业了。这不是你修复 99%的 getsync()错误的方法，很难想象这个部分会随机爆炸的情况，但是如果你正在考虑一个几乎难以解决的问题，你需要开始考虑什么是真正*不应该*失败的。

![Resonator my fix (1)](img/643de209c77ca540733f8cbaf53086b6.png)

不过，返工很棒。