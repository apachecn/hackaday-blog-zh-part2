# 一个开源的 1MHz 任意波形发生器，有一个很棒的用户界面

> 原文：<https://hackaday.com/2014/08/09/an-open-source-1mhz-abritrary-waveform-generator-with-an-awesome-ui/>

[![1MHZ DDS](img/83babac2a7dedd6d1c51b7a97dfbcadd.png)](https://hackaday.com/wp-content/uploads/2014/08/dds_tft.png)

[Herp]刚刚分享了一个[漂亮的 1MHz 任意波形发生器](http://herptronix.blogspot.fr/2014/08/tiny-dds.html)(右键- >翻译成英文，因为谷歌翻译链接不起作用)和一个设计良好的用户界面。他的平台基于 PIC32，一个带触摸屏的 [TFT 模块](http://herptronix.blogspot.fr/2013/07/open-source-smart-display.html)和 75MHz AD9834 [直接数字频率合成器](http://en.wikipedia.org/wiki/Direct_digital_synthesizer) (DDS)。当然，后者可以产生频率高达 37.5MHz 的信号…但这只是在两个输出点对你来说足够好的情况下。

正如你在下面的视频中看到的，“微型 dds”可以产生许多不同类型的周期信号，甚至可以直接在触摸屏上绘制。在 DDS 输出之后，可以使用几个运算放大器调整失调和信号幅度，并且可以使用单独的 SMA TTL 输出来使用 PIC32 PWM 信号。该平台可以读取存储在 microSD 卡上的 WAV 音频文件，还具有用于信号监控的模拟输入。广告之后请继续关注我们的视频。

[https://www.youtube.com/embed/Hllg0D2UqWg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/Hllg0D2UqWg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)