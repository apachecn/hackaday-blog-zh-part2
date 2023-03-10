# 逆向工程 Altium 文件

> 原文：<https://hackaday.com/2014/10/15/reverse-engineering-altium-files/>

在过去的几周里，我多次听到人们说，“这将是我在 Eagle 设计的最后一块 PCB。”这对 CadSoft 来说是个坏消息，但如果说 Eagle 做对了一件事，那就是他们转向了 XML 文件格式。现在，任何人都可以为 Eagle 编写自己的设计工具，而无需摆弄二进制文件。

并不是所有的 EDA 软件都是一样的，很多供应商使用二进制文件格式来保持他们的市场份额。Altium 是最糟糕的违规者之一，[但是通过深入二进制文件](http://hackaday.io/post/10390)，有可能将这些专有文件格式逆向工程成几乎人类可读的东西。

[dstanko.au]使用 Altium 文件的第一步是用十六进制编辑器打开它。是的，这是它能得到的最原始的东西，但是仅仅通过滚动文件，他就能找到一些有趣的东西。原来，Altium 使用一种叫做复合文档文件的东西，类似于 Office 用于 Word 和 PowerPoint 文件的东西，来存储所有信息。从这种文件格式的角度来看，[dstanko.au]发现所有内容都保存在一个名为“FileHeader”的流中，所有内容都是一个字符串数组(是的，所有内容都在文本中)，文本行由“|”在名称=值对中分隔。

通过一点点代码，[dstanko]设法将所有这些文本记录转储为伪纯文本格式，然后将所有内容转换为 JSON。你可以在这里查看[的所有代码。](https://github.com/dejan-stankovic/meetup-ad-schematic)