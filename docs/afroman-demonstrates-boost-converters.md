# 阿弗曼展示升压转换器

> 原文：<https://hackaday.com/2014/09/15/afroman-demonstrates-boost-converters/>

如果你需要为一个项目将电源输入调节到一个合理的电压，你可以使用开关调节器，如果不行，就使用低效的线性调节器。如果你需要提高项目内部的电压怎么办？[现在是升压转换器时间](https://www.youtube.com/watch?v=wJU7AJgERG8)，Afrotechmods 将向您展示它们的工作原理。

最简单的形式是，升压转换器仅由一个电感、一个二极管、一个电容和一个晶体管组成。通过以不同的占空比开关晶体管，能量存储在电感中，然后直接传送到电容。计算升压转换器的占空比、频率、电感和其它各种器件的值意味着一大堆数学运算，但遵循升压和开关转换器数据手册中的推荐布局一般就足够了。

![boostconverter](img/daf435ba6d8e7f326a61c619e5b53ecf.png)

本教程中的示例电路是一个围绕 LT1370 开关稳压器构建的简单升压转换器。除此之外，还有一个小稳压器、二极管、几个大电容和电阻，以及一个反馈引脚罐。这就是构建一个简单升压转换器所需的一切，连接到反馈引脚的电位计改变调节器的占空比，从而改变输出电压。

这是一种非常有效的提升电压的方式，据[阿弗曼]测量，超过 80%。它还非常容易制造，只需将少数几个零件直接焊接到一块 perfboard 上。

下面视频。

[https://www.youtube.com/embed/wJU7AJgERG8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/wJU7AJgERG8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)