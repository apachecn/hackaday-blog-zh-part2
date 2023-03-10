# 复活卡普空的歌舞伎

> 原文：<https://hackaday.com/2015/01/28/resurrecting-capcoms-kabuki/>

大约有十几个旧的卡普空街机游戏被设计成在定制的 CPU 上运行。它被称为歌舞伎，虽然大部分核心是一个标准的 Z80，但芯片的很大一部分专用于安全。当时的问题是街机板克隆，当电源从歌舞伎 CPU 上移除时，这种安全设置的内存内容丢失，游戏无法运行，20 年后，编写模拟器的人急得要命。

现在这些游戏已经有几十年的历史了，对于那些承担起保存这些旧游戏任务的人来说，歌舞伎 CPU 的片上安全性是一个问题。然而，[现在这些 CPU 可以被取消](https://www.youtube.com/watch?v=G2LEcuGLvr4)，对芯片进行编程，并将其放置在街机板中，而不会丢失其内存内容。

早些时候，我们看到了[ArcadeHacker]又名[Eduardo]为复活这些旧 CPU 所做的努力。他能够在歌舞伎上运行新代码，但要运行这些街机游戏中未经修改的原始 rom 需要硬件。现在[阿卡德哈克]有了。

该设置包括一个芯片夹，夹在歌舞伎 CPU。只需一点 Arduino 代码，原始的、未经修改的 rom 的安全密钥就可以被刷新，放入街机板(内存的内容由电池备份)，然后剪辑就可以发布了。[ArcadeHacker]这是每个街机板在工厂中的编程方式。

如果你正在寻找一个关于如何编写歌舞伎的深入的技术描述，[ArcadeHacker]在这里有一个令人难以置信的详细的 PDF 文件。

[https://www.youtube.com/embed/G2LEcuGLvr4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/G2LEcuGLvr4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)