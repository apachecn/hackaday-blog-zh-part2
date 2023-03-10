# 用这个微型 CPU 设计自学 Verilog

> 原文：<https://hackaday.com/2015/08/01/teach-yourself-verilog-with-this-tiny-cpu-design/>

如果你从未读过小说，你可能写不出一本像样的小说。学习做一件事通常包括研究在你之前其他人做了什么。试图学习新技术的一个问题是找到足够简单的东西来开始你的研究。

[InfiniteNOP]想要尝试编写 CPU，并开发了一个简单的 8 位架构，这将是一个课堂或自学的良好开端。这是一项正在进行的工作，所以可能还有一些 bug 需要处理，但是处理 bug 也可能是有教育意义的。你可以阅读[黑客](https://bitbucket.org/linuxlalala/nopcpu/src/3388fab1ca14e8642f165b3009ac4734e58ae301/HACKING?at=master)文件中的文档来了解架构的细节。简而言之，指令的最高四位编码操作，而最后四位选择寄存器操作数(有四个寄存器)。

【InfiniteNOP】用 Xilinx 工具模拟合成了 CPU，但我们觉得这可能是一个玩 [EDAPlayground](http://hackaday.com/2015/07/21/learn-fpgas-in-your-browser/) 的好借口。你可以找到一个与 EDAPlayground 一起工作的[测试平台](http://www.edaplayground.com/x/KjW)，尽管你可能想要更新 CPU 文件以匹配最新版本。

你不会想在一个真实的项目中使用这样一个简单的处理器，但是作为一个学习工具，它的大小是可以管理的。你可以以后再升级到更复杂的设计。如果你需要复习 Verilog，看看下面的视频。

[https://www.youtube.com/embed/eXb8prknDKg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent&listType=playlist&list=PLntFkFHRTxmLEv5MJN3oDvhd-5z3L5Rhi](https://www.youtube.com/embed/eXb8prknDKg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent&listType=playlist&list=PLntFkFHRTxmLEv5MJN3oDvhd-5z3L5Rhi)