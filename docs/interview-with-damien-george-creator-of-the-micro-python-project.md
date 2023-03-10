# 采访微 Python 项目的创建者[达米安·乔治]

> 原文：<https://hackaday.com/2013/11/27/interview-with-damien-george-creator-of-the-micro-python-project/>

【达米恩·乔治】刚刚创造了[微 Python](http://www.kickstarter.com/projects/214379695/micro-python-python-for-microcontrollers) (Kickstarter 预警！)，这是 Python 脚本语言的一种精简而快速的实现，经过优化可在微控制器上运行。它包括一个完整的解析器、编译器、虚拟机、运行时系统、垃圾收集器和从头开始编写的。Micro Python 目前支持 32 位 ARM 处理器，如上图所示的 STM32F405 (168MHz Cortex-M4，1MB 闪存，192KB ram)，并将在已经成功的活动结束后开源。运行 python 程序非常简单，只需将文件复制到平台(检测为大容量存储设备)并重启即可。官方的 micro python 板包括一个 micro SD 卡插槽、4 个 led、一个开关、一个实时时钟、一个加速度计，并有大量 I/O 引脚来连接许多外设。一个很好的视频可以在活动页面上找到，在休息之后嵌入了对项目创建者的采访。

*【马蒂厄】* 您好达米安，感谢您抽出时间回答我们的问题。仅仅过了几天，你的 Kickstarter 活动就已经成功了。还有 17 天，我们 期待看到活动 结束后有多少人会收到你的板子。

*【达米安】* 感谢 Mathieu/Hack-a-day 给我这个机会谈谈微 Python。我对这个项目感到非常兴奋，在活动的最初几天看到如此积极的回应真是太棒了。我尝试在 Micro Python 板中将功能性和极简主义结合起来，我真的很期待将它们发送给我所有的支持者。

*【马蒂厄】* 我们在 HaD 的感觉是，很多人可能低估了你从头开始重写 Python 脚本语言所做的工作。你花了多少时间？你能描述一下你的过程吗？

*【达米安】* 是的，需要一些时间和大量的编程技巧，才能让微 Python 适合微控制器。让我说一下，它不是 100% Python:它与 Python 3.x 有完全相同的语法，并且可以发出相同的字节码，但是库(它就是 Python)还没有全部存在。使用 Micro Python 和使用 Python 的感觉是一样的(它有 [REPL](http://en.wikipedia.org/wiki/Read%E2%80%93eval%E2%80%93print_loop) 在主板上运行)，我正在尝试让尽可能多的库工作。

我在业余时间研究微 Python 已经有六个多月了。可能已经超过 700 小时了。选择元件、设计 PCB、手工焊接零件(大部分是用热风枪——它们太棒了!),这非常有趣。)，以及编写 Python 实现本身。

Micro Python 软件最初只在我的 PC 上运行，我从一个简单的手写词法分析器开始。下一部分是解析器，编写起来很棘手，因为我希望它尽可能小(在代码中)并尽可能少地使用 RAM。我最终将语法编码在一个静态数据结构中(使用一些 C 预处理器的魔法),并编写了一个 320 行的非递归函数来动态解释这个表并解析 Python 源代码。解析器的输出是一个解析树，它被输入到编译器中。

对于编译器，我希望能够发出本机代码，以便 Python 能够在微处理器上尽可能快地运行。我需要学习如何为这一位编码 Thumb 机器指令，然后将编译器产生的堆栈机器风格的代码转换为寄存器机器风格的代码，以充分利用 RISC CPU。我还实现了一个字节码发射器和虚拟机，这样 Micro Python 可以很容易地在其他硬件上运行。

最终 Micro Python 在我的电脑上运行，然后我把它移植到微控制器上。这出乎意料地顺利，我在几天内就让它运行起来了。最初我没有内存管理器，所以它会很快在微处理器上耗尽内存，但后来我实现了一个简单的标记-清除垃圾收集器，它工作得非常好。

*【马蒂厄】* 完整的 bootloader 相关代码是自己写的吗？你使用过图书馆吗？如果是的话，是哪些？

*【达米安】* 我使用的微处理器内置了引导加载程序:这是 DFU(设备固件升级)，这意味着你只需将几个引脚保持在特定的逻辑电平并重置芯片，然后就可以通过 USB 连接进行闪存。这也使得用户无需任何特殊硬件就可以轻松升级 Micro Python 映像，并且意味着您永远无法将设备模块化。

对于板上的外设(如 GPIO 引脚和 SD 卡控制器)，我使用了标准的 STM 库，并将它们连接到 Micro Python。我还使用了由[ChaN]开发的令人惊叹的 FatFs 库来提供文件系统功能。

*【马蒂厄】* 当你开始这个项目时，你是否已经知道你需要做的一切？一路上你学到了很多东西吗？

*【达米安】* 我甚至无法开始告诉你我在做这个项目中学到了多少。我过去写过一些编程语言，包括编译成机器代码(x86)的语言，并且我有过使用许多不同微控制器的经验。但是把所有东西放在一起，从硬件到高级软件，会让你面临一系列全新的问题，你必须学会解决这些问题。比如学习如何写 USB 设备描述符，学习如何布局一个紧凑的 PCB，甚至学习 C 中新的做事方式！

你能给我们的读者推荐几篇关于如何像你一样创建一个词法分析器、解析器、编译器、垃圾收集器和虚拟机的好文章吗？

*【达米安】* 我的知识来自许多不同的地方:书本、大学课程、互联网，还有闲混。我认为实现一门语言是你能做的最令人满意的编程任务之一，而且它不一定很难。如果你想读一本书，去看看[Aho]、[Lam]和[Sethi]的《编译器:原理、技术和工具》，也被称为“龙书”。如果你只是想开始黑客，给自己设定一个实现“堆栈机器”的任务，因为这将让你对大多数部分有基本的了解。

IRC 上的一些人告诉我们，你习惯于冗长的项目，你能再多告诉我们一些你做过的其他事情吗？

*【达米安】* 我的日常工作是作为一名理论物理学家，而在这个领域你有像 LHC(大型强子对撞机)这样的项目需要 30 多年。当然，我的个人物理项目不会持续这么长时间，但从最初的想法到最终写出研究论文仍然需要几年时间。我最长的硬件项目无疑是建造我的数控机床(在 Kickstarter 视频的结尾)。为此，我设计了自己的步进电机控制板，为 Atmel micro 编写了固件来进行高级控制(不是 g 代码，但类似)，设计并建造了实际的机器(花了一年多时间…)，并编写了所有的 PC 端软件。我甚至写了一个 3D 建模程序来设计这台机器。可能是过度杀戮。

在过去的一年半时间里，我和一个朋友一起建立了一个名为[paperscape.org](http://paperscape.org/)的网站，这个网站描绘了研究论文的科学图景。这个项目最长的部分是(用 Python)实现一个 LaTeX/TeX 解析器，它可以自动提取书目信息，计算出论文是如何连接的。

我认为微 Python 是迄今为止我参与的最有趣也最具挑战性的项目。还有很多事情要做。我喜欢这个项目的一点是我从人们那里得到的反馈，以及他们关于如何改进 Micro Python 的所有建议。我期待围绕这个建立一个社区，让 Micro Python 在各种硬件上运行，做各种令人惊奇的事情。