# 自动调光器侵入键盘背光

> 原文：<https://hackaday.com/2013/05/11/auto-dimmer-hacked-into-keyboard-backlight/>

![keyboard-backlight-auto-adjustment](img/44e51247edbc21cee422044321ff96f1.png)

如标题所示，[José Faria]增加了根据环境光线水平调整键盘背光的功能。但这只是他在用这台 Razer 黑寡妇终极版进行黑客盛宴时所做的事情之一。

当他第一次收到外围设备时，他不喜欢蓝色 led 用作背光。所以他把它们都拿走，放入白色的。他对此谈得不多，但我们认为这是一大堆工作。新的颜色令人愉快，但随后调节亮度的能力开始激怒他。有四个预定义的级别，这就是你得到的。即使是有滑动条的 GUI 也不能超出这些水平。

他的解决方案是用自己的控制器来扩充控制器。他在控制 LED 电路低端的晶体管上安装了一个 AVR 芯片。同时，他还注意到键盘外壳实际上是半透明的。这让他可以在内部隐藏一个光电传感器，自动调节光线水平。但他这样做的方式仍然允许他通过开关的翻转来使用原始功能。休息之后自己看吧。

[https://www.youtube.com/embed/aUg_jtZq0TY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/aUg_jtZq0TY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)