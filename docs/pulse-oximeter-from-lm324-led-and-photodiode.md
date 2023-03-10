# LM324 的脉搏血氧仪、LED 和光电二极管

> 原文：<https://hackaday.com/2013/04/18/pulse-oximeter-from-lm324-led-and-photodiode/>

这款[脉搏血氧仪制作起来非常简单和便宜](http://www.swharden.com/blog/2013-04-14-simple-diy-ecg-pulse-oximeter-version-2/)简直就是犯罪。监控传感器输出最明显的方法是使用示波器。穷人的替身是声卡，这就是斯科特·哈登在他的文章中所展示的。

它使用了[一个我们在](http://hackaday.com/2012/11/27/pulse-oximeter-displays-blood-oxygen-levels-on-a-pc/)之前见过几次的概念。LED 发出的光穿过你的手指，在另一边由光电晶体管测量。就是你在医院里看到的病人手指上的浅灰色塑料东西。[Scott]用一个普通的木制衣夹来安装传感器，并将其与手指对齐。它由只使用一个芯片的最简单的电路监控:一个 LM324 运算放大器。他在视频中很好地解释了跳跃后的三个基本阶段。输入信号在被馈送到第一放大级之前被去耦。从那里，它被馈送到一个可调低通滤波器，以帮助消除房间内交流电源的 60Hz 噪声。最后一级使用并联的另一个低通滤波器再次放大信号。

[https://www.youtube.com/embed/bKAJsZJvMI0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/bKAJsZJvMI0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)