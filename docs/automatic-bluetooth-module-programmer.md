# 自动蓝牙模块编程器

> 原文：<https://hackaday.com/2013/09/24/automatic-bluetooth-module-programmer/>

![automatic-bluetooth-programming](img/09c9b8d0a82a48bc7f65d3f1c838b8d2.png)

在我们开始之前，不要被标题所迷惑。这不会将固件刷新到设备中。但是它确实[自动化了设置蓝牙转串行模块](http://www.reprap.org/wiki/Jy-mcu)的过程，以便在您的项目中使用。

我们经常被缺乏描述这些廉价模块的标准方式所迷惑。我们可以把它叫做 HC-05，但是我们不确定它是否正确。称之为 JY-MCU 板。如果你对差异(或缺乏)有什么看法，请在评论中告诉我们。无论哪种方式，我们都知道这些电路板可能会令人沮丧。它们可以在[各种不同的固件](http://hackaday.com/2012/01/30/firmware-programmer-for-a-cheap-bluetooth-module/)中找到，这可以使每个固件的配置过程有所不同。

[James 的]解决方案将设备连接到 Arduino，运行他写的草图。连接设备，在 Arduino IDE 中启动终端监视器，然后进行所需的设置。草图将轮询蓝牙模块，以查看它被设置为以什么速度运行。然后，它将确定主板运行的固件版本，并在终端中显示该信息。然后，它利用这些信息对电路板进行编程，使其符合您的要求。

在这种情况下，[詹姆斯]正在使用其中的一个模块来驱动他的 3D 打印机，而没有被束缚在他的笔记本电脑上。

[https://www.youtube.com/embed/WtPqC1PASQY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/WtPqC1PASQY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)