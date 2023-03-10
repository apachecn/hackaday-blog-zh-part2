# 有声读物播放器仅使用 NFC 标签进行控制

> 原文：<https://hackaday.com/2013/03/04/audiobook-player-used-only-nfc-tags-for-control/>

![no-button-nfc-audiobook-reader](img/5d053227dc139ba9fade38e9840eb93e.png)

[Martynas mickevi ius]有一位视力受损的祖母。她喜欢听有声读物，并且已经用 DVD 播放器听了很长时间了。问题是她没有办法在两次倾听之间保住自己的位置。他着手帮助建立一个没有任何按钮的专用有声读物阅读器。

这个项目的灵感来自于我们去年 11 月推出的一键阅读器。像那个项目一样，[Martynas]选择使用便宜但功能强大的 Raspberry Pi。主要区别在于控制方法。他使用的是安装在 RPi 外壳顶部的 NFC 标签阅读器。上面的图像显示了原型制作期间的装备，但他的最终版本都被捆绑在粉红色的外壳中，只需要连接电源和音频电缆。跳完之后在演示中自己看吧。

每本书都有自己的 NFC 标签。当她读完书后，她可以简单地切断电源，下次插上电源时，它又会恢复原状。标签设置是一个巨大的改进，因为它允许将整个库存储在 SD 卡上，并使用不同的标签进行选择。有了这个硬件，编写系统扩展代码应该是轻而易举的事情，比如在回放开始之前，使用文本到语音转换来宣布正在播放哪本书的脚本。

[https://www.youtube.com/embed/PfXmEMPt9ws?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/PfXmEMPt9ws?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)