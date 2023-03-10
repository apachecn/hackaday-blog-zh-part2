# 遗传算法程序员得到函数

> 原文：<https://hackaday.com/2015/01/07/genetic-algorithm-programmer-gets-functions/>

[Kory]已经写了几个月的遗传算法了。除了他让这些遗传算法做的事情之外，这本身并不是什么独特或例外的事情。[【Kory】一直用遗传算法在 Brainfuck](http://www.primaryobjects.com/CMS/Article163) 写程序。是的，是电脑给电脑编程。感谢天网晚了 18 年。

当我们第一次看到[Kory]的作品时，他已经在 Brainfuck 中编写并运行了一台计算机。虽然[Kory]选择的语言的*名*可能需要一些工作，但它实际上是计算机生成程序的理想语言。由于只有八个命令，每个命令由一个字符组成，它大大减少了任何遗传算法必须产生的和适应度函数必须评估的开销。

[Kory]最初的努力有一个缺点:功能。让一个程序说 Hello World 是相对容易的，但是要做一些复杂的事情，你需要像宏或函数这样的东西。Brainfuck，它最简单的形式，不支持函数。这给[Kory]让他的计算机编程计算机变得更聪明并克服其遗传算法中的局部极小值的计划泼了一盆冷水。

解决这个问题的方法是创造一种新的 Brainfuck 方言，叫做 BrainPlus。这采用了扩展 Brainfuck 的最佳部分，并添加了一个基本上作为 break 语句的命令。

有了这个，[Kory]的自编程计算机可以开发更复杂的程序。它已经创建了一个程序来生成斐波那契数列的前几个数字。它只会增加到 233，因为 255 是一个字节的最大值，而程序本身花了 7 个小时来生成。然而，它确实有效。用新的 Brainplus 功能生成的其他程序包括背诵墙上的 99 个瓶子和一个将两个值相乘的程序。

即使[Kory]的计算机花了很长时间来生成这些程序，如果有足够的时间，这个程序真的没有什么做不到的。Brainfuck 和[Kory]的 Brainplus 都是图灵完备的，因此给定无限的内存和时间，它可以计算任何东西。随着新功能的加入，它可以更快地计算任何东西。

[Kyle]的 GA[的所有代码都可以在 Github](https://github.com/primaryobjects/AI-Programmer)上获得。