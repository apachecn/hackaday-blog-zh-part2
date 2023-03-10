# 更多的模拟微型计算机:Stellaris 发射台上的 8080

> 原文：<https://hackaday.com/2015/04/10/even-more-emulated-microcomputers-8080-on-a-stellaris-launchpad/>

[Steeeve]刚刚把他在 Stellaris 发射台模拟一些基于 8080 的微型计算机的工作发给了我们，包括运行太空入侵者的裸机[。我们知道你在想什么:](http://programmablehardware.blogspot.ie/2014/12/space-invaders.html)[这些天你们都在做这些吗](http://hackaday.com/2015/04/08/an-apple-emulator-on-an-arduino-uno/)？！？！？[水里肯定有东西](http://hackaday.com/2015/04/07/the-dan64-a-minimal-hardware-avr-microcomputer/)。

[Steeeve]的构建基于 Launchpad，带有一个外部 64kB SPI RAM、一个漂亮的小 TFT 显示屏和一个内置 SD 卡，可满足您的所有存储需求。加上一个 8080 仿真器和一个键盘，你就有了一台微型计算机。(那是多余的吗？)

[Steeeve]项目的真正精彩之处在于，他克隆的不仅仅是一台目标计算机，而是一大堆计算机，包括(GitHub 链接如下)基于 8080 的 [UK101/Superboard](https://github.com/jscrane/UK101) 、 [CPM/80](https://github.com/jscrane/cpm80) 和运行[太空入侵者、](https://github.com/jscrane/invaders)的机器，以及基于 6502 的 [Commodore PET](https://github.com/jscrane/PET) 和 [Apple-1。另外，你可以将状态保存到内置的 SD 卡上，这样你就可以让微型计算机休眠，并在以后从你停止的地方重新开始。时髦。](https://github.com/jscrane/Apple1)

他还建立了一个[库](https://github.com/jscrane/r65emu)，如果你想自己构建这个作品，它可以提供一个仿真框架。我们提到过他会玩太空入侵者吗？好极了！