# 苹果 IIe 变成了一台 Lisp 机

> 原文：<https://hackaday.com/2013/10/20/the-apple-iie-becomes-a-lisp-machine/>

早在 20 世纪 70 年代末和 80 年代初，麻省理工学院的一些非常棒的人正在研究 Lisp 机器。这些计算机是专门为运行 Lisp 作为主要编程语言而设计的。大约在同一时间，加利福尼亚的几个史蒂夫正在开发 Apple II，它很快成为有史以来最受欢迎的电脑之一。Apple II 将 BASIC 作为其主要的编程语言，这在当时是不错的，但肯定没有 Lisp 优雅。这花了 30 多年的时间，但是亚历克斯和马丁想出了一个办法，把不起眼的苹果 IIe 变成一台 Lisp 机器。

对于这些人来说，为 Apple IIe 开发 Lisp 出奇的简单——他们只需用 C 语言编写一个 Lisp 解释器，并使用 6502 编译器生成一些机器代码。将 Lisp 移植到 Apple II 的主要问题是简单地将代码移植到 Apple II 上。我们认为，如果在 80 年代尝试过同样的项目，这可能会更容易。

为了让他们的解释器进入苹果电脑，他们使用了非常棒的 ADTPro 库，该库允许数据通过磁带端口和现代计算机的麦克风和扬声器插孔加载到 Apple II 上。在将模拟数据加载到这个数字恐龙上整整一分钟后，[亚历克斯]和[马丁]有了一个运行在古老而优雅的硬件上的 Lisp 解释器。

6502 Lisp 解释器的源代码可以在 GitHub 上找到[,以及通过现代计算机加载它的所有必要工具。那会给你所有你想要的古老的兰姆达和父母。不过，有一个警告:退格键并不完全有效，所以要做好遭受挫折的准备。](https://github.com/hausdorff/turtles)

你可以看看下面的演示视频。

[https://www.youtube.com/embed/tey9sFqICSk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/tey9sFqICSk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)