# 用你的电子游戏偷情

> 原文：<https://hackaday.com/2012/07/11/playing-footsie-with-your-video-games/>

![](img/f25873634cf0a7aaf07c7cb4d441162a.png "playing-footsie-with-your-video-games")

[Jon]将在游戏过程中用他的脚趾敲敲打打，这要归功于[这个装有按钮和传感器的脚控制器](http://blog.asdfa.net/foot-controller-v2/)。这是构建的第二次迭代。原来的一些焊点断裂，USB 停止工作。他还经历了一些不稳定的行为，所以他决定升级控制硬件，并在这个过程中增加一些东西。

这个版本使用 Arduino Uno 作为接口板。他做了大量的原型制作，以找到连接所有模拟传感器的最佳方式，以及如何正确消除按钮的抖动。一旦他对输入感到满意，他就开始寻找一种更好的方法来使用 USB HID 标准。我们很惊讶地听到 ATmega16u2(包括 USB 硬件的新型 AVR 芯片之一)不能很好地与 Linux 兼容。但是[乔恩]设法解决了这个问题，现在他用一个比以前更好的脚控器进行比赛。