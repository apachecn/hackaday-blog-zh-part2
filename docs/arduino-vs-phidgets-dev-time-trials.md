# Arduino 与 phi dgets–Dev 计时赛

> 原文：<https://hackaday.com/2015/01/04/arduino-vs-phidgets-dev-time-trials/>

在 Arduino 上开发太慢了吗？Phidgets 太贵了吗？你什么时候会使用其中的一个？hack aday regular【Ken】[分解他从三次实验性计时赛](http://kawalabo.blogspot.jp/2015/01/hardware-protoyping-speed-test-phidgets.html)中学到的东西。

Arduino 和 Phidgets 之间的主要开发差异是口味偏好和一些事实的混合。Arduino 是开源的，Phidgets 是专有的。Arduino 需要硬件和软件的混合，Phidgets 只需要(并且只允许)连接到一台完整的计算机，但支持高级语言——它有望更快更容易地完成工作。最后，Arduinos 很便宜，Phidgets 是它的 3-5 倍。

这三个计时赛是常见的任务:1 .闪烁 LED。2.用锅转伺服。3.制作一个计步器。对[Ken]来说，Phidgets 在三个实验中都赢了，但并不显著:分别是 37%、45%和 25%。只差几分钟。即使考虑时间价值，对大多数黑客来说也是得不偿失的。

[![HAD - Phidgets3](img/8265faddab38ae07c8f057de074d6892.png)](https://hackaday.com/wp-content/uploads/2015/01/had-phidgets3.jpg) 在上下文中，在最简单的项目上稍微更快速的开发的优势由于需要重建一个永久的解决方案而被浪费掉了。Phidgets 与 PC 相连，只对临时或固定项目有用。[对我们的许多读者来说，这让他们陷入了困境](http://hackaday.com/2014/05/11/the-phidgets-solar-powered-weather-station/)。Arduinos 在技术上可能是开发工具包，但足够便宜，可以作为永久的解决方案在项目中处理掉——这可能是我们大多数人的标准。

[Ken]指出，对于厌恶电子产品的软件人群来说，Phidgets 迎合了他们的喜好。Phidgets 将其昂贵的外围设备剪辑在一起，其余的都是使用熟悉的现代语言和库用代码完成的。我们想知道这个群体还能有多大；几年前，当学科之间的鸿沟更大时，Phidgets 可能是一个有趣的工具包，但这些天的趋势是每个人都对每件事都略知一二。Hackaday 的读者可能比大多数人更能代表这种趋势，但如果这种趋势似乎已经过时，请让我们知道。

[【Ken】的文章](http://kawalabo.blogspot.jp/2015/01/hardware-protoyping-speed-test-phidgets.html)对实验和平台之间的权衡做了更多更详细的解释。

如果你喜欢看平行工程，请看下面的延时视频，这是时间试验的分屏。

[https://www.youtube.com/embed/j0kXaKjxRj4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/j0kXaKjxRj4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)