# 为反激式变压器供电的简单方法

> 原文：<https://hackaday.com/2014/02/14/an-easy-way-to-power-flyback-transformers/>

![FJISRREHR3EF3OP.LARGE](img/57a4af823f3189b25c2449c406277599.png)

实话实说吧。玩高压电很牛逼。危险，但令人敬畏——嗯，只要你处理得当。反激式变压器是产生大电弧的好方法，但是给它们供电并不容易，不是吗？

首先，对于那些可能不知道的人来说，回扫变压器是老式电视和 CRT 显示器中最常见的变压器类型。它们通常可以输出 10 千伏到 50 千伏的电压——问题是，它们不那么容易供电。常见的方法包括使用晶体管式驱动器，或零电压开关([ZVS](http://en.wikipedia.org/wiki/ZVS#Quasi-resonant_zero-current.2Fzero-voltage_switch))——这就是[【Skyy】如何在 5 万伏电压下烹饪一些 s 'mores。](http://hackaday.com/2013/08/26/making-smores-with-50000-volts/)

事实证明，还有另一种更简单直接的方法。你只需要一个荧光灯镇流器。使用镇流器的输出作为反激式变压器初级绕组的输入，这可以使用万用表找到，只需找到引脚之间的最高电阻即可识别。现在，由于您正在如此高的电压下工作，您可能需要将反激式变压器浸入矿物油中进行绝缘处理，以免短路。就是这样。

现在是时候来点火花了。

[https://www.youtube.com/embed/TIKsEgtuvrg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/TIKsEgtuvrg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

如果你想变得有趣，你甚至可以用 Arduino 控制反激式变压器！