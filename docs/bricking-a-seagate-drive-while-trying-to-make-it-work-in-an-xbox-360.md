# 在试图让希捷硬盘在 Xbox 360 上正常工作的同时，对其进行砌砖

> 原文：<https://hackaday.com/2012/07/10/bricking-a-seagate-drive-while-trying-to-make-it-work-in-an-xbox-360/>

![](img/5f0f8113ec4c07cbc57168c347e24bd9.png "seagate-hard-drive-editing-for-xbox-360")

如果你想更换 Xbox 360 中的硬盘，而不仅仅是购买一个官方设备，你可能不太走运。有一个工具可以让你做到这一点，如果你用一个西方的数字驱动器作为替代品。但是，如果你的新驱动器是希捷这个工具将无法工作。[Darth Circuit] [开始让他的 Seagate 在 Xbox 360](http://darthcircuit.wordpress.com/2012/07/05/hacking-a-seagate-hard-drive-to-work-in-the-xbox-360/) 上工作，但他的手动更改最终因为一个小错误而阻塞了驱动器。

对 WD 驱动器执行此操作的工具名为 [HddHackr](http://www.xboxhacker.org/index.php?topic=11813.0) 。[达斯]通过找出程序实际上做什么开始了他的探索。为了替代原始驱动器，新驱动器必须具有相同的型号、序列号、LBA 和固件版本。一旦在二进制文件中更改了这些值，就会将其写入驱动器的特定位置。他改变了驱动器本身的这些值，并取得了相当大的进展。直到他尝试了一个新的命令，最终把他锁在了硬盘之外。现在它几乎是一块砖头，但我们希望有人能从他停下来的地方捡起来，把这项工作变成对其他人有用的东西。祝你好运！