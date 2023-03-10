# PS3 Eye 因低价而重获新生

> 原文：<https://hackaday.com/2015/05/20/ps3-eye-lives-again-thanks-to-low-prices/>

[Henry Tonoyan]已经开始涉足 OpenCV 和数字控制系统项目。他需要一个像样的网络摄像头，能够以高于标准的帧速率工作。事实证明，PS3 Eye 实际上是一个非常能干的小相机。现在它已经有点过时了，你可以从亚马逊这样的地方花 7 美元买到它！

PS3 Eye 有一个标准的 USB 接口，在 Linux 中摆弄了一下之后，[Henry]能够为他的应用程序调整帧速率设置。他使用一个名为 video for Linux 的库和一个名为 qv4L2 的应用程序。它在 VGA 下能够达到 60fps，我们承认这并不惊人，但在 7 美元的价格下，我们不能抱怨——如果你降到 QVGA (320×240)，你可以达到 120fps。

从那里，您可以尽情地在 OpenCV 中玩耍。

鉴于 Eye 已经问世 7 年多了，它已经在相当多的黑客中使用过。从一个真实的眼球追踪器([认真地说](http://hackaday.com/2010/12/11/kids-type-with-their-eyes-robot-arm-prints-their-words/))，到一个带有触摸追踪的[互动投影地球仪](http://hackaday.com/2014/01/22/interactive-globe-is-awesome-for-google-earth/)，甚至[一个实体塔防游戏。](http://hackaday.com/2011/08/31/multitouch-tower-defense-uses-physical-towers/)