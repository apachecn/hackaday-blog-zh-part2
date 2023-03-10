# AVR 芯片的宏汇编

> 原文：<https://hackaday.com/2012/12/12/macro-assembly-for-avr-chips/>

![avr-macro-assembly](img/514882fddf41515780edca8ab7ed6590.png)

这里有一个有趣的提示，可以帮助您提高编写汇编代码的能力。为了消除 AVR 项目汇编代码的复杂性，[Quinn Dunki]想出了用 GNU 工具链编写 AVR 代码时如何使用宏。任何使用 AVR-GCC 的人都应该记住这一点，如果他们想要或者需要用汇编语言来完成一个项目的话。

如果你看上面的代码片段，你会看到两个明显不是汇编的命令；PulseVRAMWrite 和 DisableVRAMWrite。这些宏指令指导汇编程序滚入一大块代码。但是这个工具链使用的汇编器 avr-as 缺乏处理宏的能力。这太糟糕了，因为我们同意[Quinn]的观点，即这些宏使代码更容易阅读，并大大降低了打字错误的概率，因为宏中的代码将被重复使用。

答案是修改 makefile 文件以使用 [GNU M4](http://www.gnu.org/software/m4/) 。我们没有听说过它，但毫无疑问它已经安装在我们的 Linux Mint 系统上了(更多信息请参见 man m4)。这是一个强大的宏处理器，它根据一个定义宏的独立文件来交换她的所有宏。结果是一个汇编文件，将播放 avr-as 很好。

她的实现是为了帮助她的 Veronica 计算机项目开发[GPU。](http://hackaday.com/2012/04/10/veronica-gets-vram-and-its-own-boot-logo/)