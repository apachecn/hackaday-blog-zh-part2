# 书虫玩 Bot 考验程序员 OCR 技能

> 原文：<https://hackaday.com/2014/03/24/bookworm-playing-bot-tests-programmers-ocr-skills/>

![bookworm-bot](img/d6120ca400e71e7919ddd6a2e81f233f.png)

看看这个聪明的机器人，它的[Jari]被提升到[统治书虫豪华记分牌](http://sol.gfxile.net/bookworm/)。该机器人运行在 win32 机器上，拉截图来看游戏板，模拟鼠标点击来玩。跳跃后的视频显示，它像冠军一样比赛，但它花了一些时间才能走到这一步，[Jari]花时间分享所有的开发细节。

编写这些类型的机器人最困难的部分是识别游戏部件。看看上面静止镜头中的所有动画…很多瓷砖都模糊不清，有不同的颜色，当机器人拼写并提交每个单词时，瓷砖本身也会移动。

经过反复试验后，Jari 选定了一个图像预处理器，它将像素值相乘四次，然后用 1/6 的阈值查看每个像素，为每个瓷砖生成一个黑白面。从那里，一点光学字符识别比较每个瓷砖与一组已知的例子。这非常有效，导致了编程挑战的逻辑和字典部分。

你认为这比珠光宝气的闪电战机器人容易还是难？那一个是寻找特定的像素区域，这一个基本上是一个集中的滚动你自己的 OCR 脚本。

[https://www.youtube.com/embed/VEuNhNdbY44?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/VEuNhNdbY44?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)