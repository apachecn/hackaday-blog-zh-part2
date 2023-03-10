# 对唱针进行逆向工程

> 原文：<https://hackaday.com/2012/07/22/reverse-engineering-a-stylophone/>

60 年代的音乐玩具 Stylophone 是一件非常简单的工程作品。通过一个简单的金属键盘和一支唱针以及几个晶体管，Stylophone 能够产生一些不可思议的时间声音，相当于电子音乐领域的前斯特拉迪瓦里小提琴。[Simon] [拆开了一个原装的唱针](http://www.waitingforfriday.com/index.php/Reverse_Engineering_the_Stylophone)，彻底拆了电路，仔细研究了为什么这个古老的音箱如此酷的来龙去脉。

已经有相当多的 DIY Stylophone 克隆品，但它们都遭受了由 555 定时器芯片[发出的同样刺耳的声音，稍微被误导的制造商使用了](http://hackaday.com/2010/09/23/analog-stylophone/)而不是原版中使用的张弛振荡器(如上图所示)。除了振荡器连接到金属键盘的 RC 电路外，[西蒙]还研究了颤音电路。这只是一个产生 8 赫兹正弦波的简单振荡器。当然，键盘通过一组电阻连接到电路上，西蒙很乐意为这些电阻提供值。

[西蒙]放了一张他的逆向工程唱针的原理图，让你可以克隆这个古老的电子乐器。如果你能找到晶体管的话。