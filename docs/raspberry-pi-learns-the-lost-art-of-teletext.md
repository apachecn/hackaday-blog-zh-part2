# 树莓派学会了失去的文字电视艺术

> 原文：<https://hackaday.com/2013/07/07/raspberry-pi-learns-the-lost-art-of-teletext/>

![rpi-teletext](img/ad045c263763ccb52770ba2085ed678c.png)

探索死协议往往是爱好电子产品爱好者的名片。为什么不呢？错误已经犯下并被改正了——你可以从中吸取教训。这个 [Raspberry Pi 图文电视黑客](http://thenewtech.tv/tech-life/teletext-revival-part-2-making-it-work)就是一个完美的例子。它让[月光]探索生成复合视频的领域，以及在 Raspberry Pi 和微控制器之间建立通信。

图文电视是在计算机网络普及之前，通过电视获取信息的一种方法。这在当时是非常令人印象深刻的，你可以从[这个复古的特征](http://hackaday.com/2012/08/21/retrotechtacular-1983s-answer-to-information-overload/)中得知。[月光]开始研究通过简单地用 AVR 芯片产生 PAL 信号来重建图文电视设备。他遇到了一个设备故障(记住，这是*总是*一个硬件问题),形式是一个伪造的复合 USB 加密狗。在更换了接收设备后，他开始运行并准备探索协议的细节。正如你所看到的，他的成功甚至让他旋转了一个分线板，插入 RPi GPIO 头。Y 形分离器(连接器？)将 RPi 的合成输出与来自他自己的板的覆盖数据相结合。