# 适合各种场合的 RGB LED 显示屏

> 原文：<https://hackaday.com/2014/04/03/blinkenschild-the-rgb-led-display-for-every-occasion/>

![turd](img/45d5a2d923d0225ee28ff9cc15e90572.png)

一天早上，他决定抗议欧洲议会对马排便权的立场，这是一项可追溯到查理大帝时代的珍贵自由。最好的方法当然是[闪烁灯](http://hackaday.io/project/363-Blinkenschild)。他称他的项目为 Blinkenschild，这是我们见过的最好的便携式 LED 显示屏之一。

[显示屏](https://metalab.at/wiki/Blinkenschild)基于大约 15 个 RGB-123 LED 面板，每个面板包含 8×8 矩阵的 WS2811 LEDs。那是 960 像素，全部由一个小小的 3.1 英寸控制。电力由 15 个并联在一起的脂肪电池提供，给他 6 Ah 的电池寿命。笨重，是的，但它足够小，可以放在背包里，这就是(埃弗弗洛)坐在那里的东西。

显示器的动画是由 [Glediator](http://www.solderlab.de/index.php/software/glediator) 生成的，不幸的是，这是一个用于 LED 矩阵的非开源控制应用程序。Glediator 通过串行端口发送数据，但不通过 IP 或直接发送到文件中。不想随身携带笔记本电脑，[overflo]创建了一个虚拟串行端口，并将 Glediator 的输出转储到一个文件中，这样它就可以被存储在 SD 卡上的~~回放~~，并由 Android 应用程序控制。非常聪明，这正是提高人们对马和互联网关注的事情。

下面视频。

**更新:** [在下面的评论中查看【艾佛洛】的澄清](http://hackaday.com/2014/04/03/blinkenschild-the-rgb-led-display-for-every-occasion/comment-page-1/#comment-1327004)。

[https://www.youtube.com/embed/VX14pmky07Q?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/VX14pmky07Q?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)