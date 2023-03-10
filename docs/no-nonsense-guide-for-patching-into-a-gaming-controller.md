# 没有胡说八道的游戏控制器修补指南

> 原文：<https://hackaday.com/2013/07/13/no-nonsense-guide-for-patching-into-a-gaming-controller/>

![patching-into-a-gaming-controller](img/2f157d2402ef13a060739ea2a85a4388.png)

这里有一个直接的指南，指导[如何点击大多数游戏控制器](http://makezine.com/projects/hack-a-video-game-controller-for-greater-accessibility-or-cheating/)上的按钮。为什么要做这样的事？嗯，我们的目标一直是[通过机器学习](http://hackaday.com/2013/04/14/teaching-a-computer-to-play-mario-seemingly-through-voodoo/)征服马里奥。但是我们希望这将进一步激励黑客贡献他们的时间和专业知识[为残疾人开发专门的控制器](http://hackaday.com/2013/06/20/building-custom-game-controllers-for-people-with-physical-disabilities/)。

在这个例子中，一个通用的 NES 仿制控制器为所有的控件获得一个突破头。在仔细检查内部的 PCB 后，可以清楚地看到，这些按钮只是将一条线路短路到了地面。通过在每个按钮的活动迹线和母接头之间焊接跳线，控制器仍然可以正常使用，或者可以通过微控制器注入按钮按压。

上面看到的 Arduino 通过将一个引脚拉低来模拟按钮按压。从这里你可以开发更大的按钮、脚踏板，或者甚至是一些基于头部运动或其他适应性技术的[软件命令。](http://hackaday.com/2013/07/05/playstation-3-contolled-with-head-movement/)

[https://www.youtube.com/embed/jF4luAnFYgQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/jF4luAnFYgQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)