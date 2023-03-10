# 树莓派暂停然后接住…嗯，暂停

> 原文：<https://hackaday.com/2015/08/25/raspberry-pi-halt-and-catch-well-halt/>

从我们记事起，就一直有黑客攻击、利用和对未记录的 CPU 指令的好奇。Z80 拥有它们。甚至 HP41C 计算器也有一些未记录的代码。HCF(停止并着火)指令是虚构的，但我们总是听说旧的视频控制器芯片可以被哄骗炸毁某些显示器。最近你不会听到太多类似的事情，也许是因为越来越少的人使用汇编语言。

[Sergiàlvarez I Capilla]不仅从事汇编语言工作，他在编写 ARM 汇编程序时注意到了一些有趣的事情。指令是按常规模式构建的，但有些模式丢失了。怎么办？抓紧时间尝试它们。

他的结果？他发现至少有一条指令可以让树莓派死机。这本身没什么大不了的，但是指令没有受到保护，所以任何用户程序都可能锁定 Pi。当然，重置会让事情恢复正常。没有燃烧发生。顺便说一句，新型号似乎是免疫的，[Sergi]测试了一些带有 ARM 处理器的手机和其他设备，但没有效果。

实际影响？大概不多吧？但是如果你把一个 Pi 放在一个临界系统中，你可能会发现这个结果很有趣。也许对这种攻击最好的防御是[只有一个以](http://hackaday.com/2011/07/27/building-a-one-instruction-computer/)开始的指令。顺便说一下，6502 是众所周知的有大量有用的未记录的操作码。在下面的视频中有一些关于这一点的讨论(未记录的部分大约在 6:00 开始)。

[https://www.youtube.com/embed/_aSc6IlI-iM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/_aSc6IlI-iM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)