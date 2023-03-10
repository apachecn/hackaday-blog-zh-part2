# 基于音频的 USB 示波器和信号发生器，售价 20 美元

> 原文：<https://hackaday.com/2014/05/27/an-audio-based-usb-oscilloscope-and-signal-generator-for-20/>

![SoundScope](img/05660e4e3d3ba1863128422ce93771be.png)

你有兴趣花 20 美元，不费吹灰之力就造出一个 [20kHz 双通道示波器和一个双通道信号发生器](http://www.instructables.com/id/USB-Oscilloscope-with-Signal-generator/)吗？一定要看看[Jana Marie 的] Instructable，它讲述了如何从一个便宜的 USB 声卡构建这个令人敬畏的工具。

我们在过去已经展示了[吨](http://hackaday.com/2013/07/08/arduino-oscilloscope-at-five-megasamples-per-second/)和[吨](http://hackaday.com/2012/07/14/android-oscilloscope-built-from-parts-just-laying-around/)的 DIY 示波器，但这次努力的结果是一些很好地组合在一起，同时保持非常简单易懂和易于制作。你甚至根本不需要修改 USB 声卡。这个版本最酷的部分之一是你可以从你的 USB 声卡上拔下你的探针组件，并把它带到你被黑客攻击的任何地方。构建完成后，你所需要的就是[【克里斯蒂安·蔡特尼茨的】声卡示波器](http://www.zeitnitz.de/Christian/scope_en)程序，你就可以开始了。使用基于音频的示波器时，经常被忽略的一个主要缺点是它是“交流耦合的”。这意味着您不能使用声卡测量低频(包括 DC 信号)。请务必听从[Jana]的建议，不要将内置声卡用作示波器。没有保护电路，它肯定会烧坏你的电脑。

你围绕音频接口做了哪些[模拟项目](http://hackaday.com/2012/07/02/decoding-rf-link-using-a-pc-soundcard/)？我们已经看到这样的界面用于许多不同的应用，包括一些有趣的[医疗](http://hackaday.com/2008/05/26/make-an-ecg-with-your-sound-card/)相关的[黑客](http://hackaday.com/2013/04/18/pulse-oximeter-from-lm324-led-and-photodiode/)(一定要把安全放在第一位)。写信告诉我们吧！