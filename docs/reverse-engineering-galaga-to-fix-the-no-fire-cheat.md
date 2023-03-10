# 逆向工程 Galaga 修复无火作弊

> 原文：<https://hackaday.com/2015/04/11/reverse-engineering-galaga-to-fix-the-no-fire-cheat/>

我们不知道加拉加有诈，但(克里斯·坎特雷尔)知道。因此，他做了任何好奇的黑客都会做的事情——对游戏进行逆向工程，以诊断并最终修复漏洞。

剧透啊喂！如果你想按照[克里斯]的逆转努力的实际发生顺序，先去看看网站。

故障是由首先杀死大部分蜜蜂引发的。当只剩下六个时，它们进入第二种模式，在那里它们掠过屏幕并环绕边缘。俯冲时，有时蜜蜂会在 X=0 的坐标上开火。现在两个事实:在任何给定的时间，屏幕上最多有八枚导弹，X=0 的位置是软件保留的，用来隐藏不需要更新的精灵。

最终的结果是八枚导弹卡在一个永远不会掉的地方，不会被抽中。在整个游戏中没有进一步的射击。你赢了。

这就是笑点，但是每个人都知道一个好的笑话就在讲的过程中。如果你真的对学习逆向工程感兴趣，去读读[Chris]的解释，然后自己解决它们。

这是我们电脑考古的通用插头:

运行在 MAME 或类似模拟器上的古代视频游戏是学习逆向工程的绝佳场所；你可以暂停机器，在内存中翻转一点，然后观察接下来会发生什么。当时内存也很贵，所以游戏本身很小。(这不像试图对微软 Office 的所有插件进行逆向工程。)旧芯片的汇编语言很小，也有很好的文档，而且大多数时候你也有一个很好的编译器。你还能要求什么？

一个穿越教程？我们刚刚给了你一个。

哦还有 PS: [如果你过了 255 级](http://donhodges.com/galaga_stage_256_fix.htm)，游戏就抓狂了。

[https://www.youtube.com/embed/XkAqfhGNc9o?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/XkAqfhGNc9o?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)