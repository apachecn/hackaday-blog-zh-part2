# 运行带音频的任天堂 DS 未签名代码

> 原文：<https://hackaday.com/2014/12/31/running-nintendo-ds-unsigned-code-with-audio/>

即使你没有撕掉原来 DS 的顶部屏幕来创造一个更好的 Game Boy Advance，这个旧的硬件仍然可能有一些生命。[Smea] [在任天堂 DS](https://www.youtube.com/watch?v=zEd4Vw2bmBE) 上运行未签名的代码，只使用廉价游戏和一个音频文件。

这一次的漏洞利用形式可能是任何曾经在 Wii 上安装过家酿频道的人都熟悉的。像 SmashStack 一样，这个漏洞利用在游戏中使用了关卡编辑/转移功能，这次是用 6 年前的 DS 游戏 [Bangai-O Spirits](http://en.wikipedia.org/wiki/Bangai-O_Spirits) 。

[smea]正在使用基于声音的电平传输功能将未签名的代码加载到 DS 中。这种电平转换功能的工作原理是发送一个具有给定振幅的 1024 赫兹的单周期正弦波；二进制 1 比二进制 0 大几个 dB，并且由于缓冲区溢出，可以将代码加载到 DS 中并跳转到该代码。没有冗余，没有纠错，这不是你在 DS 上加载未签名代码时想要的东西。然而，它确实有效。

github 上提供了为这个漏洞[生成音频有效载荷的代码，如果你有 Bangai-O Spirits 的副本，你可以通过](https://gist.github.com/smealum/dbc3c04ca8224410d60a)[播放这个文件](http://smealum.net/soundhax.wav)来亲自尝试一下(耳机警告)。

谢谢[gudenau]的提示

[https://www.youtube.com/embed/zEd4Vw2bmBE?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/zEd4Vw2bmBE?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)