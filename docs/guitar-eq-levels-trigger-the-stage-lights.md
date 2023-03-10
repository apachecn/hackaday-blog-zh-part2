# 吉他均衡器水平触发舞台灯光

> 原文：<https://hackaday.com/2013/04/11/guitar-eq-levels-trigger-the-stage-lights/>

![guitar-eq-strobe-control](img/19377f7c60180fb29c3491bd4a061966.png)

即使你的乐队还没有成名，上演一场精彩的演出还是很有意思的。这个软件将帮助你在表演中增加灯光效果，而不必花钱请灯光技术员。[Phil]做了一个黑客程序，让你用脚踏开关设置音量阈值[来触发灯光。](http://www.unmaintained.com/index.php/eqtrigger-triggering-lights-with-guitar-equalizer-levels/)

在阅读了关于[为踏板](http://hackaday.com/2013/04/02/an-eq-display-for-a-pedal-board/)增加 EQ 显示器的黑客之后，他有了将概念转换为控制硬件而不仅仅是反馈的想法。就像可视化项目一样，他使用了负责音频分析的 MSGEQ7 芯片。他用这个做电吉他，所以他只用 Arduino 监听三到四个输出。他通过在外壳的盖子上安装一个瞬时按钮，将硬件安装到脚踏板中。踩下按钮会使 Arduino 保存当前的音量。每当它再次达到那个阈值，它就会接通电源继电器来驱动插座。在这种情况下，当他开始摇滚时，闪光灯就会打开，这就解释了上面这幅奇怪的图像。休息之后，你可以通过观看剪辑来更好地感受戏剧效果。

[https://www.youtube.com/embed/m05eCJA6ZM0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/m05eCJA6ZM0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)