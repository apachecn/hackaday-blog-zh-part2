# 基于 Excel 的高频晶体管放大器计算器

> 原文：<https://hackaday.com/2014/07/31/an-excel-based-high-frequency-transistor-amplifier-calculator/>

[![amplifier calculator](img/4fe75ebf6546d83c8e74e9d83e9a6e35.png)](https://hackaday.com/wp-content/uploads/2014/07/screen1.png)

[Paulo]刚刚向我们透露了他制作的基于 Excel 的[高频晶体管放大器计算器](http://paulorenato.com/joomla/index.php?option=com_content&view=article&id=127:high-frequency-transistor-amplifier-calculator&catid=4:projects&Itemid=4)。我们猜测我们的一些读者已经熟悉这些[A 类放大器](http://www.electronics-tutorials.ws/amplifier/amp_5.html)，通常用于放大小音频信号。忽略它们的效率相当低的事实——它们制造成本低，不需要很多元件，通常是向新的电子爱好者介绍晶体管的好方法。你通常需要做的就是[一些计算](http://www.electronics-tutorials.ws/amplifier/amp_2.html)来正确设置你的输出信号，然后你就可以开始了。

然而，当您放大 200MHz+信号时，事情会更加复杂，因为必须考虑所有元件(复数)阻抗，这样才能获得一个良好的放大系统。另一方面，在这些频率下，传输线路阻抗甚至可能会因沿途 SMT 焊盘上残留的焊料和助焊剂量而异。[Paulo]的计算器因此将计算两个 A 类共发射极/集电极放大器在特定负载下的大部分特性。