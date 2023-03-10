# 界面控制和显示拆卸

> 原文：<https://hackaday.com/2014/04/07/piface-control-display-tear-down/>

![PIFace4](img/24bb3f41c9d006785f204d8878b8b6a3.png)

[John's]目前正在进行一项相当有趣的 PiNoir & Santa Catcher 挑战赛，其中一个主要组件是 PiFace 控件和显示器，它允许您在没有键盘或鼠标的情况下使用树莓 Pi。好奇想知道这个模块是如何工作的，[John] [决定做一个拆卸](http://shropshirelug.wordpress.com/2013/12/30/piface-control-display-tear-down/)来找出答案！

他使用脱焊工具拆除了遮挡面板上大多数组件的 16×2 LCD，露出了微芯片 MCP23S17 的 16 位 SPI 端口扩展器。他继续检查元件，并用万用表检查数值，得出以下电路图:

[![PiFace+Control+and+Display](img/6aad8f9079978bc25d3a30b2db771e16.png)](http://hackaday.com/wp-content/uploads/2014/04/pifacecontrolanddisplay.png)

Click to Zoom

这是逆向工程中的一个很好的练习，看起来[约翰]做得相当不错。我们已经看到了用于自动倒酒瓶的 PiFace，使用物理红石控制《我的世界》，甚至使用由 48 个 Pi face、Pi 和摄像机组成的阵列进行 3D 成像。