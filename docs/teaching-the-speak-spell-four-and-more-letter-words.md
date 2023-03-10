# 教授朗读和拼写四个(或更多)字母单词

> 原文：<https://hackaday.com/2012/12/03/teaching-the-speak-spell-four-and-more-letter-words/>

![ss](img/604e5b716c2a6b0c0547fded119d5c7e.png)

在成为全世界电路弯曲者的宠儿之前，Speak & Spell 是现代技术的一个奇迹。配有微处理器和语音合成器，Speak & Spell 能够说出有限的词汇，这些词汇[furtek]认为应该包括诸如“基地组织”、“坏死”和“屁股”等词。Speak & Spell 包括一个扩展端口，用于容纳更大词汇量的墨盒，并花了很大力气创造了自己的 Speak &法术车，让它能像水手一样说话。

语音和拼写只读存储器存储在一个非常奇怪的存储芯片上。在返回保存的数据之前，芯片一次读取 5 个字节，而不是并行或串行接口。起初，[furtek]认为他可以得到一个 ATtiny 微控制器，但这种存储芯片的设置方式使得它甚至无法在 400kHz 的 I2C 总线上发送和接收数据。

该项目最终找到了一些像样的硬件，即基于 CPLD 的盒式磁带，它的速度足以与 Speak & Spell 接口。在那之后，唯一的问题就是用一些旧的 Windows 3.1 软件将单词转换成 speech synth 可以理解的东西，最后烧一张 ROM。

最终的结果是一个带有反常词汇的咒语，比一个有几根电线交叉的电路弯曲的硬件有趣得多。休息之后请看视频。

[https://www.youtube.com/embed/JngcLfVQT5U?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/JngcLfVQT5U?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)