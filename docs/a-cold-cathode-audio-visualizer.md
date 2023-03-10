# 冷阴极音频可视化仪

> 原文：<https://hackaday.com/2013/08/07/a-cold-cathode-audio-visualizer/>

![CC](img/89b116ed33f71b3a732448a7ac08e193.png)

最后，冷阴极灯不仅仅可以用来照亮你的电脑内部，或者让你的鞭子看起来像可以悬浮一样。[詹姆斯]发现如果他改变进入逆变器的电压，只有一定量的灯管会发光。给一个黑客一个有趣的观察和足够的时间，最终他会想出一些非常酷的东西。在这种情况下，[它是一个冷阴极音频可视化器](http://www.youtube.com/watch?v=8JM6bj8RyEo)，由荧光灯管供电，做着意想不到的事情。

构建细节有点不足，但我们能够哄出[詹姆斯]构建的 imgur 专辑。他正在使用[这 20 盏 CCFL 灯](http://www.xoxide.com/20-front-bar-blue.html)，用 TDK·CCFL 逆变器替换了库存的数字逆变器。

这个建筑的数字控制由一个 Arduino Mega 和一个定制的防护罩提供。我们猜测图形均衡器由 MSGEQ7 芯片提供，逆变器本身通过 Mega 的 PWM 引脚供电。这很像一个 9 英寸的谢妮图形情商，只是大得多。[詹姆斯]正在计划这个版本的更大版本，称为 Mega speKtrum，我们已经迫不及待地想看到这个版本以及适当的报道。