# 斐波那契时钟很难读，看起来不错

> 原文：<https://hackaday.com/2015/05/07/fibonacci-clock-is-hard-to-read-looks-good/>

数百年来，艺术家们一直在他们的作品中融入黄金比例，人们认为当比例符合这一比例时，往往更具美感。考虑到这一点，[Philippe]创造的时钟在数学上必须是我们曾经展示过的最好看的时钟，即使很难从中辨别时间。

时钟由代表斐波纳契数列前五个数字的方块组成。这些方块由 led 背光照明，红色代表小时，绿色代表分钟，蓝色代表小时和分钟的重叠。简单地将红色和蓝色方块相加得到小时，将绿色和蓝色方块相加得到分钟。分钟以 5 分钟为增量显示，因为没有足够的块，所以你也必须相乘。困惑了吗？如果不是，那么使用这种方法有几种显示特定时间的方法，其中任何一种都可以由时钟随机选择。[Philippe]报告说，例如，6:30 有 16 种不同的表示方式。

时钟由 ATmega328P 驱动，装在一个木箱里。在[Philippe]的网站上有原理图和代码，如果你想建造自己的时钟，这里有如何用这个时钟报时的详细说明。你可能需要这些。如果你喜欢被时钟弄糊涂，你可能也会喜欢这个。

[https://www.youtube.com/embed/ridpWzFKS3I?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/ridpWzFKS3I?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)