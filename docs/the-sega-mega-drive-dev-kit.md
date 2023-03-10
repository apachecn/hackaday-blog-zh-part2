# 世嘉大型驱动开发套件

> 原文：<https://hackaday.com/2014/06/18/the-sega-mega-drive-dev-kit/>

虽然大多数自制视频游戏开发都集中在最初的 NES、雅达利游戏机上，并制作了一些 SNES 游戏，但还有一种游戏机并没有受到太多的喜爱。世嘉的经典控制台，创世纪或兆驱动，取决于你从哪里来，是一个非常强大的机器，在当时具有惊人的能力。[Chris]认为 Mega Drive 将成为一体化开发套件的良好目标，通过大量工作[他成功地将一个整合在一起](https://www.youtube.com/watch?v=mEH7a-a8dvQ)。

Genesis 或 Mega Drive 的标准盒式磁带只是一个简单的 ROM 芯片，直接连接到控制台的地址空间。[Chris]用一个便宜的 FPGA 和一些双端口 ram 在现代世界和这个古老的主机内部之间创建了一个无缝接口，允许他从 SD 卡上加载每一个 Mega Drive 游戏，并使用现代工具修改旧游戏，甚至创建新游戏。

为了展示他的开发工具包，克里斯复制了索尼克 1，并使用调试器和 GDB，给了自己无限的生命。这是一个非常酷的演示，使用标准的 Linux 调试工具搜索由 Megadrive CPU 执行的所有命令。通过跟踪，[Chris]找到了减少代表 Sonics 寿命的值的指令，用 NOPs 替换它，实际上给了自己无限的寿命。这很像游戏精灵的工作方式，只是使用了好得多的工具。

当然，如果 USB 开发工具包只能修改现有的游戏，它就没有多大用处。[Chris]工作的真正力量来自于能够开发自己的演示、游戏和自制应用程序。

[Chris]需要使用 [SGDK](https://code.google.com/p/sgdk/) 为他的开发套件的 ROM 加载器部分编写一个小型的自制 Mega Drive 应用程序。[用开发工具包反汇编他自己的代码](http://www.youtube.com/watch?v=dLoudQc8L08)，他能够看一看指令，甚至可能修改他的加载器。

这是一项令人印象深刻的技术成就，对于 Mega Drive 来说，这可能是一个非常小的自制领域的福音。所有的电路板、代码和其他东西都可以在[Chris]的 github 上的[上获得，整个项目](https://github.com/makestuff/umdkv2)[都写在 hackaday . io](http://hackaday.io/project/1507-USB-MegaDrive-DevKit)的上。视频如下。

[https://www.youtube.com/embed/mEH7a-a8dvQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/mEH7a-a8dvQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/JxBzxhMhANI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/JxBzxhMhANI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/dLoudQc8L08?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/dLoudQc8L08?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)