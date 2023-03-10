# 使用 Newlib 和 Stellaris Launchpad

> 原文：<https://hackaday.com/2012/12/18/using-newlib-with-stellaris-launchpad/>

![using-newlibc-with-stellaris-launchpad](img/648f725813359f8600caa0d3171d61c0.png)

[Brandon]通过演示如何将 newlib 与 TI Stellaris Launchpad 一起使用，将我们带入了更深的层次。这是他在关于[使用 GCC 和 ARM 硬件](http://hackaday.com/2012/12/04/a-study-of-gcc-and-the-ti-stellaris/)的帖子中构建的框架的一个很好的延续。但是它肯定比第一篇文章更复杂。

使用 newlib 而不是 glibc 提供了编译 C 代码的选择，这些代码包括为计算机编码时常见的系统调用，但在嵌入式系统中很少见。由于与 printf 相关的开销，通常避免使用类似的东西。但是这些处理器变得如此之快，拥有如此之多的内存，这在某些情况下可能是有用的。在开发 STM32 贪吃蛇游戏时，我们简单地考虑过实现 malloc 来创建一个链表。[Brandon]在这里的工作使该命令的使用成为可能。

该过程从为栈/堆的开始和结束添加标签开始。这使得函数分配内存成为可能。考虑到链接器脚本的变化，你必须实现一些系统调用函数，比如 _sbrk。