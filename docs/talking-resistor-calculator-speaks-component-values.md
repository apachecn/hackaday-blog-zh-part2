# 发声电阻计算器发声元件值

> 原文：<https://hackaday.com/2012/06/11/talking-resistor-calculator-speaks-component-values/>

![](img/ad85bdc52fa20ed0b883cd62313a7e92.png "resistor")

如果有一件事肯定会蒙蔽我们，那就是读取电阻色带。更糟糕的是，红色看起来与橙色一模一样，棕色和黑色难以区分，不同的元件制造商出于某种原因不会使用相同的涂料来为其电阻编码。[Jeff]Gadget guggar 也有同样的问题，所以他做了一个[会说话的电阻计算器](http://www.gadgetgangster.com/news/56-jeffs-shop/548-talking-resistor-calculator.html)来告诉他电阻值。

构建的电子部分非常简单，只需一个提供 12 位分辨率的 MCP3208 ADC。软件方面是这个项目真正的亮点。[杰夫]使用了一个装有视差推进器的[小工具强盗快速启动板](http://www.gadgetgangster.com/find-a-project/56.html?projectnum=258)。8 个内核并行运行，螺旋桨足以运行【菲尔·皮尔格林】的[软件语音合成器](http://forums.parallax.com/showthread.php?89411)。当一个电阻连接到两个鳄鱼引线时，螺旋桨通过查找表找到一个与来自 ADC 的数字相匹配的电阻值。从那里，它只是发送一串语音文本到语音合成器对象。

尽管文本到语音转换芯片已经问世几十年了，[Jeff]还是选择用软件来构建他的语音合成工具。这可能只是对 Propeller 微控制器的强大功能的一个证明，但任何能让我们不盯着电阻色带的东西对我们来说都没问题。