# 通过远程入侵亚马逊 Echo

> 原文：<https://hackaday.com/2015/07/18/hacking-amazon-echo-through-its-remote/>

这太疯狂了…实际上是一个电子设备在和另一个电子设备对话。在英语口语中。这很有效。

我们已经报道了亚马逊 Echo 的几个黑客攻击，但有些人可能会惊讶地发现，它还附带了另一个有趣的硬件——遥控器。给它装上一个树莓皮，你就给自己找到了一种自动控制回声的方法，而无需拆开回声本身。[Gamaral]做到了这一点，并为他的 Echo 提供了一些显著增强的功能。

他从识别遥控器的电源轨开始。然后，他接入一个 3.3v 电压调节器，并使用一个 100 欧姆的电阻作为分压器，将其降低到 Echo remote 使用的 1.8 伏逻辑电平。一根单线从 Raspi GPIO 连接到控制器上的一个触觉开关。

对于软件，Raspi 运行的是带有 Espeak 的 RPi buildroot 和编译的 cron 调度程序。这使得他可以向 Echo 发送命令，让它说任何他想说的话。但是 Echo 接受的任何语音命令都应该有效。如果你想走出这些界限，看看[我们前几天看到的欺骗 WeMo 设备的方法](http://hackaday.com/2015/07/16/how-to-make-amazon-echo-control-fake-wemo-devices/)。

请务必查看下面的[gamaral]娱乐视频，看看黑客的行动。

[https://www.youtube.com/embed/9Ilw0f4srE8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/9Ilw0f4srE8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)