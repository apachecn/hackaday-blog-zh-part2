# 破解编辑器:编程字体

> 原文：<https://hackaday.com/2015/09/02/hack-an-editor-fonts-for-programming/>

我们最近注意到两种面向程序员的不同字体，每一种都有不同的编辑器定制方法。第一个， [Fira Code](https://github.com/tonsky/FiraCode) ，透明地将常见的编程符号转换成单个字符。例如，<——变成了箭和！=(或者< >)变成了一个适当的不等于号。另一种字体， [Hack](http://sourcefoundry.org/hack/) (不能与名称争辩)，旨在使常见的混淆字符清晰可见。例如，零字形与字母 o 的外观非常不同。

很容易理解 Hack 是如何工作的，但 Fira 起初似乎是个谜。你的 C++编译器期望，但是屏幕显示一个箭头。

一旦你安装了字体，你仍然需要告诉你的编辑器使用该字体，但是这是几乎每个 IDE 都有的设置(即使你必须在某个地方编辑一个配置文件)。我们对 Fira 代码喜忧参半。它有一个很酷的因素，但它也让人觉得你在隐藏实际的代码，这似乎不是一件好事。

如果你想推出自己的字体，有很多方法可以创建字体。自然地，你甚至可以用一个网络应用程序来做这件事(见下面的视频)。当然，如果你做了[我们希望听到它](http://hackaday.com/submit-a-tip/)。

[https://www.youtube.com/embed/Jow2qPLP74A?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/Jow2qPLP74A?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

感谢[k5rud]指出 Hack。