# 在 Hackaday 上开发的:有时，你所需要的只是一些标志

> 原文：<https://hackaday.com/2014/10/01/developed-on-hackaday-sometimes-all-you-need-is-a-few-flags/>

Hackaday 社区[离线密码管理员](https://github.com/limpkin/mooltipass)的开发到现在还不到一年。自 7 月以来，我们的测试人员一直在努力工作，给我们不断的建议，关于他们希望看到实现的功能和开发团队可以做出的改进。这导致了超过 1100 次 GitHub 提交和一万行代码。正如你所猜测的，我们小小的 8 位微控制器的闪存很快就被填满了。

我们的贡献者之一[Miguel]最近发现了一个编译和一个链接器标志，这使我们在 26KB 固件上节省了大约 3KB 的闪存存储，而几乎没有增加处理开销。抓紧你的帽子，这篇报道会变得很专业…

来自全球各地的许多编码人员同时在 Mooltipass 固件上工作。根据他们想要实现的功能，会为他们分配一个专用文件夹。从逻辑上讲，它们产生的代码根据所需的任务被分成许多 C 函数。这增加了 GCC 编译器通常使用*调用*汇编指令进行的许多函数调用。

这个特殊的 8 位指令使用一个 22 位长的值，该值包含要调用的函数的绝对地址。因此，每个函数调用总共使用 4 个闪存字节(不传递参数)。不过， [AVR 指令集](http://www.atmel.cimg/doc0856.pdf)还包含了另一种方式，通过使用[相对寻址](http://en.wikipedia.org/wiki/Addressing_mode#PC-relative)来调用函数。这条指令是 *RCALL* ，使用一个 11 位长的值，包含当前[程序计数器](http://en.wikipedia.org/wiki/Program_counter)和要调用的函数之间的偏移量。这将函数调用减少到 2 个字节，并减少了一个时钟周期。因此， -mrelax 标志使我们通过让链接器开关*尽可能调用带有 *RCALL* 指令的*来节省 1KB。

最后，*-mcall-prologes*编译器标志释放了 2KB 的闪存。它创建在程序例程开始和结束时调用的主[序言/结尾](http://en.wikipedia.org/wiki/Function_prologue)例程。简而言之，在执行任何功能之前，它以相同的方式准备 AVR 堆栈和寄存器。这将因此浪费[一点点执行时间](https://github.com/limpkin/mooltipass/pull/129)，同时节省大量代码空间。

点击[此链接](http://www.tty1.net/blog/2008/avr-gcc-optimisations_en.html)可以找到更多节省空间的技巧。想继续关注 Mooltipass 的发布日期吗？订阅我们的[官方谷歌群](https://groups.google.com/forum/?hl=en#!forum/mooltipass)！