# 打字机打字，播放音乐

> 原文：<https://hackaday.com/2015/06/27/typewriter-types-plays-music/>

做了一个梦。他想把打字机改装成打印机。当然，[以前也做过，](http://hackaday.com/2015/04/21/ascii-art-with-pure-data-and-a-typewriter/)但是【克里斯】想创造他自己的版本。他拿起一台 60 年代的史密斯电晕电动打字机，希望用电脑驱动它的按键开关。你可以想象当他发现钥匙根本不是电开关，而是一个复杂的机械系统，触发离合器撞击实际纸张时，他有多惊讶。意识到这不是一个简单的布线工作后，[Chris]将这个项目搁置了几年。

与塔夫茨大学的同事[Bruce Molay]的一次谈话重新点燃了[Chris]对这个项目的兴趣。[Bruce]建议使用螺线管来按键。[Chris]一头扎进去，很快就有了 48 个螺线管。第一个问题是在按键上安装螺线管。[克里斯的]室友碰巧是[德里克·西伯里]，Artisan 的庇护黑客空间的总裁。[德里克]创造了一个丙烯酸框架，它可以容纳螺线管，并直接安装在打字机的键盘上。这意味着不需要对打字机本身进行修改。只需抬起螺线管阵列，你就可以像 1965 年一样摇滚了。

下一步是驱动所有这些螺线管。为此，克里斯与他在塔夫茨大学的学生[凯特·瓦辛楚克]一起工作。[Chris]使用德州仪器 [TPIC6A595](http://www.ti.com/product/tpic6a595) 移位寄存器设计了一块电路板。TIPC“电源逻辑”系列工作起来像常规的 74 系列逻辑，但有严重的输出。这些芯片可以处理高达 50 伏和 1.5 安培的脉冲输出电流——对于[Chris'] 24 伏螺线管来说足够了。[Chris]自学 Eagle 中的原理图输入和 PCB 布局。仅仅试了两次，他就有了一个来自[奥什帕克](https://oshpark.com/)的工作板。

Arduino Uno 将 USB 上的串行输出转换为准备输入移位寄存器的位流。在电脑方面，[Chris]编写了一个基本的 CUPS 驱动程序，允许他从 Macbook 上打印。这个项目的完美演示结果是音乐。点击休息时间观看史密斯·科罗纳演奏勒卢瓦·安德森的“打字机交响曲”。这可能是这首特别的音乐第一次用真正的单词来演奏，而不是随机的按键。

[https://www.youtube.com/embed/iL4rsxR5GnI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/iL4rsxR5GnI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/le4C2HeNrdQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/le4C2HeNrdQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

这是“打字机交响曲”的经典版本

[https://www.youtube.com/embed/wZCh4EY_kug?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/wZCh4EY_kug?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)