# 带括号的 Python

> 原文：<https://hackaday.com/2014/02/10/python-with-braces/>

![python](img/a9ebc7824d2b72898b41c616fd38d5b5.png)

如果 Python 有一点让人有点不安的话，那就是完全没有大括号，或者像美国英语中所说的吊带。大括号是各种 C、Java、PHP、Perl 和一大堆其他非常强大的语言的一个特性，它使内容更加易读，并且不依赖于精确的缩进。[Ruby]和[Eran]在一个项目中提出了一种在 Python 中使用这些标点符号的方法，他们称之为[带括号的 Python](http://www.pythonb.org/)。

顾名思义，带大括号的 Python 不关心缩进:你可以自由地让你的代码变得极其丑陋，或者以 K&R 风格恰当地编写你的代码。每行以分号结束，只有一条语句的代码块不需要花括号，就像 C 和 Java 一样。

现在[Ruby]和[Eran]已经有了一个带有 OS X 软件包的 Windows installer。执行带大括号的 Python 脚本只需要用‘Python b’可执行文件执行，而不是普通的‘Python’可执行文件。