# 失落的 ROM 的袭击者

> 原文：<https://hackaday.com/2014/09/14/raiders-of-the-lost-rom/>

曾几何时，街机风靡一时。你可以带着满满一口袋的硬币去当地的游戏厅，尝试许多不同的游戏。如今，电子游戏厅不那么受欢迎了。因此，许多旧的街机游戏变得越来越难找到。它们几乎就像古代的人工制品。随着时间的推移，它们会慢慢腐烂，经常丢失或被遗忘。进来吧，MAME。

MAME(多街机模拟器)是一个软件项目，其目标是通过防止这些街机丢失或遗忘来保护游戏历史。MAME 模拟器目前支持超过 7000 个标题，但仍有更多的需要保存。致力于保护这些游戏的黑客就像世界上的数字印第安纳·琼斯。他们了解丢失的游戏，并寻找保存它们。在某些情况下，为了准确地保存内容，他们必须避开安全措施。没有什么比滚动的巨石或毒镖更可怕的了，但还是很安全。

许多由出版商 NMK 生产的拱廊橱柜使用了一种特殊的声音处理器，标签为“NMK004”。该芯片包含一个受保护的内部代码 ROM 和一个控制声音硬件的不受保护的外部 ROM。实际的音乐数据存储在一个单独的未受保护的 EEPROM 中，每个游戏的音乐数据都不相同。系统从 EEPROM 读取音乐数据，然后使用 NMK004 内部的秘密数据进行处理。

围绕内部 ROM 的安全措施一直在防止黑客倾倒其内容。结果是，使用这种芯片的 NMK 游戏在使用 MAME 时模拟的声音很差，因为没有人知道原始芯片是如何处理音频的。[trap15]发现 20 年过去了，没有人试图绕过安全措施，转储 ROM，这很可笑。他把事情掌握在自己手中。

整个故事有点长，包含几个曲折，但它很值得一读。精简版是经过大量的试错和编写许多定制工具后，[trap15]终于能够转储 ROM 了。他能够使用一个非常聪明的技巧来完成这个任务，这个技巧被其他人推测过，但是从来没有在这个硬件上尝试过。[trap15]利用在未受保护的外部 ROM 中发现的漏洞，欺骗系统回放受保护的内部 ROM，就好像它是存储在 EEPROM 中的声音数据一样。该系统将读取内部 ROM，就好像它是一首歌，并通过扬声器播放出来。[trap15]将生成的音频以 WAV 文件的形式录制回他的电脑。然后，他必须编写一个自定义工具，将 WAV 文件解码成可用的数据。

[trap15]已经发布了他所有的工具和文档，因此其他黑客可以使用它们进行自己的硬件黑客冒险。这个项目花了很长时间，是逆向工程和毅力的一个很好的例子。

[谢谢瑞安]