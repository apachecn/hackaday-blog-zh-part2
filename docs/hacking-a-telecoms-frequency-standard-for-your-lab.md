# 为你的实验室破解电信频率标准

> 原文：<https://hackaday.com/2015/07/23/hacking-a-telecoms-frequency-standard-for-your-lab/>

[Shane Burrell]偶然发现了一个北电 GPSTM，并将其重新用作他的实验室的 10MHz 参考。GPSTM 被设计成嵌入背板，最有可能用于电信应用。所以[谢恩]需要黑掉主板来运行 48v PSU。一旦加电，它相对容易接口，因为卡似乎包含众所周知的 Trimble Thunderbolt 模块，并与其软件兼容。

在之前，我们已经介绍过[频率参考](http://hackaday.com/2013/08/26/making-a-hp-frequency-counter-more-accurate/) [，它们对实验室来说是很有价值的补充。在大多数示波器、频谱分析仪和函数发生器的背面，您会发现一个 10MHz 参考输入，允许用户提供比内部产生的参考更精确的参考。外部参考不仅通常更准确，还可以让您的所有设备与公共参考保持同步，这在某些测量中尤为重要](http://hackaday.com/2014/09/15/low-cost-lab-frequency-reference/)。虽然一些黑客选择铷源，但北电设备中的 GPS 纪律温控振荡器应该提供一个不错的稳定参考。

不过，给[谢恩]一个警告，沉迷于黑客频率参考，你可能会成为一个[时间迷](http://leapsecond.com/time-nuts.htm)发现自己爬山去[测试相对论](http://www.npr.org/templates/story/story.php?storyId=17345235)。

[https://www.youtube.com/embed/tB-E5FPVvwU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/tB-E5FPVvwU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)