# 火神 74:复古工程的杰作

> 原文：<https://hackaday.com/2015/08/11/vulcan-74-a-masterpiece-of-retro-engineering/>

[激进的布拉德]已经玩过 FPGAs，视频信号，并且在他的简历上已经有一些惊人的项目。现在他疯了。[他正在 6502.org 论坛上记录一台计算机的构建](http://forum.6502.org/viewtopic.php?f=4&t=3329),这台计算机只有 65C02、几个 SRAM 芯片和一大堆逻辑芯片组成，具有 Amiga 质量的图形。

这个项目的设计目标是用大约 1980 年的零件和图形建立一个领先十年的视频游戏系统。视频输出为 VGA，分辨率为 400×300，绚丽的八位色彩。这个项目中唯一比移位寄存器更复杂的芯片是一个 65c02 和几个(现代的)15ns SRAMs。这在 80 年代早期是不可能的，但是唯一的阻碍就是那个时代缓慢的 RAM 芯片。

到目前为止，[Radical]已经完全用 74 系列逻辑构建了一个 GPU，它可以读取 RAM 的一部分，并将其转换为 XY 位置、颜色、像素和 VGA 信号。有对阿尔法通道和多个精灵的支持。计划是增加声音硬件，支持四个独立的数字频道和 1 兆字节的样本存储器。这是一个令人惊讶的雄心勃勃的项目，当你意识到他在无焊试验板上做所有这些时，它会变得更加令人印象深刻。

[布拉德]将继续更新 6502.org 的线程，直到他完成或尝试死亡。到目前为止，看起来很有希望。他已经有了一堆在显示器上蹦蹦跳跳的球。你可以看看下面的视频。

[https://www.youtube.com/embed/M9kUlFZM0gM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/M9kUlFZM0gM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)