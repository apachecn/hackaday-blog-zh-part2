# 新零件日:忆阻器

> 原文：<https://hackaday.com/2015/07/02/new-part-day-memristors/>

在过去的几年里，知情人士一直对忆阻器感到好奇。对忆阻器的最简单解释来自其名称本身——它是一个*记忆电阻器*。实际上要复杂一点，但这一基本理解足以说明这样一个事实，即它是一个电阻，根据流过它的电流大小来改变电阻。忆阻器最初是在 70 年代由[Leon Chua]描述的，这个想法在期刊上发表了近 40 年，2008 年惠普实验室创造了一个工作中的忆阻器。

[现在可以买一个](http://www.bioinspired.net/products-1.html)。实际上，您可以购买 8 个 16 引脚 DIP 封装。据报道，这款 16 针 DIP 售价 240 美元。每个忆阻器只要 30 美元，这是你第一次可以买到它们。

这些忆阻器基于银硫族化物(Ge2Se3)。当电路“写入”这个忆阻器并施加正电压时，银离子迁移到硫族化物，形成数据手册( [PDF](http://nebula.wsimg.com/6dba75009009af7a59036365876b3f66?AccessKeyId=64577CB1C10F8DCEF8A3&disposition=0&alloworigin=1) )中所说的树枝状晶体。这降低了忆阻器的电阻。当向器件施加负电压时，这些树突被移除，忆阻器被“擦除”，并且忆阻器返回高阻态。

这种银硫族化物忆阻器不同于惠普实验室开发的氧化钛忆阻器，当谈到这种被遗忘的电路元件时，氧化钛忆阻器是最常被引用的。这项工作来自博伊西州立大学的克里斯蒂·坎贝尔。她已经为此工作了十多年，拥有 [IEEE 出版物](http://ieeexplore.ieee.org/xpl/abstractAuthors.jsp?tp=&arnumber=4616863&url=http%3A%2F%2Fieeexplore.ieee.org%2Fxpls%2Fabs_all.jsp%3Farnumber%3D4616863)、[会议论文集](http://scholarworks.boisestate.edu/electrical_facpubs/73/)(那一个的全文)、[和几十项专利](https://www.google.com.ar/patents/WO2003019691A3?cl=en&dq=ininventor:%22Kristy+A+Campbell%22&hl=en&sa=X&ei=reuUVcf4AoOo-QGS5IGIBg&ved=0CCMQ6AEwAQ)。

至于忆阻器的应用，通常有两个学派。就目前的计算机技术而言，最有趣的是存储。忆阻器可以在 NAND 闪存或老式磁性硬盘驱动器的一小部分空间中保存二进制 0 或 1。这意味着更高的存储密度、更大容量的硬盘和更低的功耗要求。这些忆阻器有循环次数的限制，根据数据表，“超过 2000 次”。这比 MLC 闪存少了近一个数量级，这是磨损均衡无法合理补偿的。不过，这是一项新技术，所以这种情况可能会改变。

忆阻器的第二个主要预期用途是神经网络。神经网络只是一系列的输入、一些神经元、输出以及三者之间的连接。这些连接是加权的，忆阻器的可变电阻使它们处于一个独特的位置，可以在最基本的硬件上模拟曾经用软件和定制 asic 完成的事情。这些忆阻器的商品名——Neuro-Bit——和公司名称——Bio Inspired Technologies——给你一个预期用途的线索。

正如所有的新技术一样，总有一些东西是不可避免地被创造出来的，而这些东西是最初的设计者从来没有想到过的。这些新的应用是什么目前还只是推测。既然任何人都可以买到这种精巧的新芯片，那么看看用这些部件能做出什么将会很有趣。