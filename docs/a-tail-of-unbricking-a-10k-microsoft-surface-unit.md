# 一个(拆卸)价值 1 万美元的微软 Surface 设备的故事

> 原文：<https://hackaday.com/2012/06/29/a-tail-of-unbricking-a-10k-microsoft-surface-unit/>

![](img/08470760f8c6e08dc45faef0b53e7719.png "microsoft-surface-unbricking")

当一个硬件停止响应时，我们都有过这种沮丧的感觉，以及“我刚才是不是用砖砌了这个东西？”我们脑海中的火箭。[Florian Echtler]最近在极端情况下经历了这一点，因为他对慕尼黑大学的微软 Surface 2.0 的黑客攻击导致它无法响应。他说这是一个 8000 欧元的硬件，相当于大约 10000 美元！显然，他的首要任务是让这东西重新运转起来。

那么，如果你得到这样一个硬件，你应该做的第一件事是什么呢？当然，试着在上面运行 Linux。而[Florian] [很轻松地做到了这一点](http://floe.butterbrot.org/matrix/hacking/surface/)(休息之后有一个快速的概念验证视频)。他拿了一个为不同目的编写的 Linux 内核驱动器，并将其修改为与 MS Surface 接口。在发现一些错误信息后，他把它打包并调用到 good。过了一段时间，该部门打电话给他，询问他的 Linux 内核工作是否与显示器死机有关。呀。

他深入研究了驱动程序，发现一个 bug 可能导致了 USB 接口芯片上的固件被覆盖。最大的问题是他们不只是为这个芯片发布图像。因此，他最终不得不转储 EEPROM 中剩余的内容，并逐字节重建报头。

[https://www.youtube.com/embed/e-JNqTY_3b0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/e-JNqTY_3b0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)