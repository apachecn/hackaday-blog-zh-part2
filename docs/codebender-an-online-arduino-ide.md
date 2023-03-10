# Codebender:一个在线 Arduino IDE

> 原文：<https://hackaday.com/2012/07/01/codebender-an-online-arduino-ide/>

因为一切都在向网络应用转移，[Vasilis Georgitzikis]，又名[tzikis]开发了 [codebender](http://codebender.cc/) ，这是一个基于云的 Arduino IDE，其中充满了内置库、文档和从浏览器向 Arduino 上传代码的能力。

为了编译一个 Arduino 草图，codebender 使用了 [clang](http://clang.llvm.org/) 一个非常棒的编译器，它会给你关于可怕代码的非常描述性的警告。像任何好的 IDE 一样，它有内置的高亮显示和文档，一小部分 Java 允许你上传你的代码并在浏览器中监控串口。

更有趣的创新之一是 codebender(即将推出)使用 TFTP 引导加载器。有了这个和一个以太网盾，就可以很容易地将代码上传到任何一个联网的 Arduino 上，不管它是在你的桌子上还是在地球的另一边。我们可以看到它对数据记录器甚至无人机气球非常有用，我们迫不及待地想看到它的实际应用。