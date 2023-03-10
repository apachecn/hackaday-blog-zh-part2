# μJ，一种用于微控制器的 Java 虚拟机

> 原文：<https://hackaday.com/2012/10/15/%ce%bcj-a-java-virtual-machine-for-microcontrollers/>

![](img/bc3677e800b951b21f1f9d89878c8d25.png "mammal")

[Dimitri]提交了一个他一直在做的项目，即[完全用 C 语言](http://dmitry.co/index.php?p=./04.Thoughts/11.%20uJ%20-%20a%20micro%20JVM)实现了一个 Java 虚拟机，并且可以在微控制器之间轻松移植，例如我们通常看到的 AVR 和 PICs、ARM 设备，甚至是低级的 386。

在“如何做”之前，[Dimitri]首先解释了为什么他想在微控制器上运行 Java 字节码。基本上，他发现现有的解决方案，如 Arduino 环境，对于只想对芯片编程的人来说太复杂了。Arduino 和 PICAXE 需要类似 C 的语法和指针；当每个人和他们的母亲都能用 Java 编程时，这可不是件容易的事。

至于[Dimitri]如何设法将一个 JVM 打包到一个微控制器中，那完全是另一回事了。JVM 中的一切，从 double、long 和 float 数据类型到异常，整洁的线程相关函数如“synchronize ”,甚至方法如 String.charAt()和 String.length()都是完全可选的。如果你的微控制器太小，就禁用你不需要的功能。

至于μJ 运行得有多好，多快，[Dimitri]展示了一个 ATMega644 和 PIC24 运行他的 JVM 和一个小的 Java 应用程序的演示。您可以在休息后查看这些视频，或者在[Dimitri]的网站上下载μJ 的源代码。

[https://www.youtube.com/embed/-gaXtCXLrxk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/-gaXtCXLrxk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent) [https://www.youtube.com/embed/iFzg9y2saac?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/iFzg9y2saac?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)