# JavaScript 中的多普勒手势检测

> 原文：<https://hackaday.com/2015/03/13/doppler-gesture-sensing-in-javascript/>

[Daniel]无意中发现了一篇有趣的论文([，我们在](http://hackaday.com/2012/03/21/doppler-effect-lets-you-add-gestures-to-your-computer/)之前报道过)，关于仅使用计算机的扬声器和麦克风进行多普勒手势感应。不幸的是，这篇论文没有包括源代码，所以【丹尼尔】[用 JavaScript 创建了自己的多普勒手势感应](https://danielrapp.github.io/doppler/)实现，可以在浏览器中正常工作。

【丹尼尔】的 [JavaScript 库](https://github.com/DanielRapp/doppler)产生一个 20 千赫的正弦波，通过电脑的扬声器播放。频率很高，几乎听不见。当音调通过扬声器播放时，计算机的麦克风用于对音频进行采样并计算信号的频谱。在播放音乐时，当你把手靠近电脑时，接收信号的频率会变高；当你移开你的手，它会变得更低。[丹尼尔]的脚本寻找这种频率偏移，并使用它来触发事件。

![doppler](img/36dfe08d7046df14508d3586cfce6fea.png)

[Daniel]在他的网站上有一些很棒的例子，你可以自己测试一下它的功能。他有一个不用手的滚动例子，频谱图，甚至还有一个虚拟的特雷门琴。由于他的代码被打包成一个易于使用的库，所以应该很容易集成到任何网页中。该库唯一真正的限制是，它目前只能在 Chrome 上工作(Firefox 不支持禁用回声消除)。