# 老鹰捉小鸡:给差异添加意义

> 原文：<https://hackaday.com/2013/09/04/git-with-eagle-add-meaning-to-diff/>

我们喜欢 Git。我们知道每个人都有自己喜欢的版本跟踪工具。但是即使那些不关心 Git 的人也应该看到[从跟踪 Eagle 布局文件](https://github.com/nerdy-works/Geagle)中获得有意义的 Diff 数据的价值。

最后那句话对你来说只是胡言乱语吗？让我们后退一步。几年前，Eagle 根本不可能使用版本控制，因为原理图和 PCB 布局软件通常将其文件保存为二进制文件。但是后来 [Cadsoft 过渡到将 Eagle 文件保存为 XML](http://hackaday.com/2010/10/14/cadsoft-eagle-migrating-to-xml/) 。这为像[脚本这样的东西打开了大门，它们可以一起重命名部件](http://hackaday.com/2013/01/18/renaming-parts-in-eagle-cad-by-editing-the-xml-directly)，并在版本控制下跟踪文件。后者的一个问题是，对一个文件的两个不同版本执行 Diff 会导致 XML 更改，而这些更改可能是人类不可读的。[帕特里克·弗兰肯]写这个剧本至少是为了增加一丝意义。

我们希望在原理图或电路板效果图上看到并排突出显示。但如果我们真的看到它，那还很遥远。现在，他的脚本将接受 Diff 并打印出上面看到的表格，表示从一个版本到下一个版本做了哪些类型的更改。这是一个开始，我们希望它能激发这个领域更多的工作。