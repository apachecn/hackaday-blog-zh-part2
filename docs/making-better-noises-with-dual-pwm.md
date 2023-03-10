# 利用双 PWM 产生更好的噪声

> 原文：<https://hackaday.com/2013/01/17/making-better-noises-with-dual-pwm/>

![pwm_16b_sm](img/1ca0177bad7899f0d56373ca5676a81a.png)

虽然在 ATMega328 上获得 16 位分辨率在技术上是可能的，但在每个人最喜欢的“Mega ”(包括几乎每个 Arduino 草图)上的大多数 PWM 实现都仅限于 8 位 PWM。这意味着引脚只能输出 256 个不同的值，所以如果你在玩 Arduino 上制作的音乐，不要期望非常高的保真度。

有一个巧妙的解决方法:使用两个 PWM，一个引脚用于高字节，另一个引脚用于低字节。[这就是开放音乐实验室在从事需要高质量音频的合成器项目时所做的](http://www.openmusiclabs.com/learning/digital/pwm-dac/dual-pwm-circuits/)。

构建背后的基本思想是 PWM 引脚可以用来产生音频。使用两个 PWM 引脚并将它们相加意味着可以增加额外的分辨率位。这需要在每个引脚上使用不同的电阻值。例如，在两个 PWM 引脚上使用相同阻值的电阻可以将分辨率提高一位。电阻值比为 1:4 的两个引脚将分辨率提高了 4 位，依此类推。

在 ATMega 或 Arduino 上设置这些更高分辨率的双 PWM 输出有一个很好的教程,以及针对这种双 PWM 设置的[失真分析](http://www.openmusiclabs.com/learning/digital/pwm-dac/pwm-distortion-analysis/)。