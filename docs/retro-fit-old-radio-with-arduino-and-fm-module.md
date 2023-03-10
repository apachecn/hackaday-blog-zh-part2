# 用 Arduino 和 FM 模块改造旧收音机

> 原文：<https://hackaday.com/2015/07/02/retro-fit-old-radio-with-arduino-and-fm-module/>

俗话说:“不能把新酒装在旧瓶子里”。但是，如果你是一名黑客，却被一台 2005 年制造的收音机困住，你就会明白了，这台收音机看上去像是用 1975 年的技术组装的。[马库斯·詹金斯]就这么做了，从他的旧收音机中取出内部零件，将其转换成一个 [Arduino FM 收音机](http://marcusjenkins.com/hardware/arduino-fm-radio/)。

他那便宜的市电收音机调谐很差。它在定位站点时遇到了困难，并且倾向于漂移。一看内部，很明显它的设计一点也不好，所以任何修复它的尝试都是没有意义的。相反，他绘制了一个简单的原理图，使用了 Arduino Nano、基于 TEA5767 的 [FM 无线电模块和基于 LM386 的音频放大器。](http://www.ebay.com/sch/items/?_nkw=tea5767&_sacat=&_ex_kw=&_mPrRngCbx=1&_udlo=&_udhi=&_sop=15&_fpos=&_fspt=1&_sadis=&LH_CAds=&rmvSB=true)

Arduino 上的一个按钮有助于在存储在内存中的预设频率范围内循环。Arduino 通过 I2C 连接到调频收音机模块。现有天线连接到 TEA5767 模块。收音机模块输出立体声音频，但[Marcus]满足于只使用单声道，因为这将在他的工作室中使用。音频放大器非常简单，基于数据手册中的[典型应用。尽管焊接调频收音机模块有点棘手，但他还是把它们都组装到了原型板上。Arduino 代码非常简单，可以从](http://www.ti.com/lit/ds/symlink/lm386.pdf)[下载](http://marcusjenkins.com/wp-content/uploads/2015/06/garageRadio.zip) (zip 文件)。

他保留了原来的调谐旋钮，但现在已经不能用了。AM-FM 选择器旋钮配有一个连接到 Arduino 的微型开关，用于选择预设电台。里面的几乎所有东西都是用(马库斯)所谓的“热鼻涕”胶水粘在一起的。整个练习花了他几欧元，零件是从他的零件箱里捡出来的。一台好的收音机可能只需花几欧元就能从旧货市场买到，而且花费更少，但那不会像这台一样酷。

深入探究一下[FM 信号是如何调制解调播放的](http://hackaday.com/2014/06/26/the-basics-of-frequency-modulation/)。