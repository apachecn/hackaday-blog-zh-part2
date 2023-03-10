# 完全集成的 HiFi 演播室监视器

> 原文：<https://hackaday.com/2014/02/13/fully-integrated-hifi-studio-monitor/>

![Studio Monitor and PCB](img/fee52094db9e75814cf932147b94fae4.png)

你有没有想过建立一个高品质的音频交叉和放大器？[Rouslan]花了很多心思让他的[双放大器录音室监听](http://rdimitrov.info/blog/show.php?entry=Minimalistic%20HIFI%20Bi-Amplified%20Speaker%20System)既高质量又易于制造。

有了简明的原理图、有意义的框图和仿真结果，他写得很好的帖子拥有你需要的一切，来基于德州仪器的 [LM4766](http://www.ti.com/product/lm4766) 构建自供电双安培扬声器。很高兴看到验证电路功能的仿真，当使用复杂的模拟滤波器和音频电路时，这将大有帮助。对于那些没有 PSPICE(一种昂贵的专业仿真工具)的人来说，[Rouslan]使用了来自 Linear Technology 的 [LTspice](http://www.linear.com/designtools/software/#LTspice) 。[德州仪器的 TINA-TI](http://www.ti.com/tool/tina-ti) 是另一个很棒的免费替代品。

此外，[Rouslan]讲述了双放大器录音室监听系统的典型问题，如相位失调和开启爆音，然后提供了解决方案。请注意，他的项目由 20VAC 供电，这需要一个外部变压器来将墙上的 120VAC 转换为 20VAC。小心高压！将来，增加一个高质量的电压调节器很可能会提高性能。

他的文章以一个非常干净的电路板结束，这是他从奥什公园订购的。有了这样一个完整的设计，没有什么可以阻止你建立自己的。走出去，好好利用你地下室里的老扬声器吧！

如果你身边没有老演讲者，看看这些非常酷的 DIY [音箱](http://hackaday.com/2011/03/04/audio-two-fer-sneaker-speakers-and-diy-mid-fi-woofers/)。