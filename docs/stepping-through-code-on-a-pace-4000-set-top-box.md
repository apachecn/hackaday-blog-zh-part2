# 在 Pace 4000 机顶盒上单步调试代码

> 原文：<https://hackaday.com/2014/09/19/stepping-through-code-on-a-pace-4000-set-top-box/>

[李]写信告诉我们他黑了一个机顶盒。在有线电视行业的律师们亮出他们的火焰剑之前…他没有偷有线电视，或者真的做了什么。这是一个黑客只是为了冒险和刺激，使别人的硬件设计做你的命令，没有任何指示。

他分两部分发布了这次冒险经历。第一步是[找到 JTAG 头](http://www.sodnpoo.com/posts.xml/pace4000_jtag.xml)并识别引脚。Arduino 来救援了！不，真的，这是我们喜欢的 Arduino 使用类型。使用[一个叫做 JTAGenum](https://github.com/cyphunk/JTAGenum/) 的软件包，该板成为探测和识别 JTAG 连接的快速工具。

上图显示了不同的硬件。从外观上看，我们很确定这是一个专门为 ARM 处理器的 JTAG 调试设计的总线增强器。这是他的文档的第二部分的开始，其中[涉及代码转储和使用 OpenOCD 和 GDB 单步调试代码](http://www.sodnpoo.com/posts.xml/pace4000_display_hack_over_jtag.xml)(或指令)。跟踪[李]发现的一切只是为了在盒子的显示屏上写下他的名字，这是一件苦差事。但是我们确实发现它很有趣。该显示器具有复杂的寻址方案。我们假设有级联移位寄存器驱动这些段，这就是为什么它会有这样的行为。自己看看吧，在评论中告诉我们你的想法。