# 不使用任何字母或数字编写 Javascript

> 原文：<https://hackaday.com/2012/08/13/writing-javascript-without-using-any-letters-or-numbers/>

![](img/89b4d1562923fc0d38269c13a27455d9.png "javascript-without-letters-or-numbers")

您知道不使用任何字母或数字也可以编写 Javascript 代码吗？不仅仅是 Javascript，这也是本演示中使用的语言。[Patricio Palladino]向[展示了如何只用八个字符](http://patriciopalladino.com/blog/2012/08/09/non-alphanumeric-javascript.html)编写代码，而且它们都是标点符号。

类型转换是这个游戏的名字。从一个由一对方括号组成的空数组开始，[Patricio]可以通过将数组转换为加号来生成数字 0。从那里，他可以使用感叹号(布尔型)和加法来生成任何数字。上图是数字 0-9 的一个例子。对于较大的数字来说，这将变得非常乏味，但还有另一个捷径。将数字转换成字符串，将它们连接起来，然后再转换成一个数字，就大功告成了。

这种技术令人着迷，基本上不可读。作为概念的证明，他编写了一个解析器，可以将任何 Javascript 转换成这种象形文字。查看[他的 Github 库](https://github.com/alcuadrado/hieroglyphy)来试一试。

[via [Reddit](http://www.reddit.com/r/programming/comments/xzs1z/write_any_javascript_code_with_just_these/)