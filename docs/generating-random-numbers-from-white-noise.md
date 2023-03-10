# 从白噪声生成随机数

> 原文：<https://hackaday.com/2012/09/12/generating-random-numbers-from-white-noise/>

![](img/37cae93be5b4b12419d395d725da5214.png "noise")

尽管 rand()对于制作视频游戏来说可能是一个足够好的随机数生成器，但它产生的随机位模式可能不足以满足需要真正随机数据的应用程序。[Giorgio] [建造了自己的随机数生成器](http://holdenc.altervista.org/avalanche/)，经过多次统计测试后，它对于一些非常复杂的计算来说足够随机。

之前，我们看到[Giorgio]用[Chua 电路](http://hackaday.com/2012/08/24/generating-truly-random-sequences/)生成随机数，但是尽管构建电子奇怪吸引子很复杂，实际上有一个更简单的随机数据来源:白噪声发生器。

[Giorgio]为这个项目设计的随机数发生器只是一对电阻、一个运算放大器缓冲器、放大器和电流开关，用于将模拟数据转换为随机 1 和 0 的数字输出。[Giorgio]通过将数字插头插入 Raspberry Pi 的一个 GPIO 引脚来采集数据，并用一个小脚本记录数据。

为了验证他的比特序列实际上是随机的，[Giorgio]对数据进行了一些测试，一些测试在确定随机性方面比另一些更可靠。

因为每个项目都需要一些令人惊叹的可视化效果，[Giorgio]在位图中将每个比特序列绘制成黑色或白色像素[。最终的图像当然*看起来*像电视静态图像，所以数据没有明显的问题。](http://holdenc.altervista.org/avalancimg/bitmap_seq1_108000000_500us.png)

[Giorgio]还用他的兆字节随机数据进行了一次有趣的蒙特卡罗模拟:通过在平面上绘制点(范围从 0，0 到 1，1)，[Giorgio]可以通过测试一个点是否在半径为 1 的圆内来近似π的值。使用 10，000 点随机数据得到的圆周率的最佳近似值是 3.1436

当然，[Giorgio]让他的随机数据通过了一些适当的统计测试，如 rngtest 和[die harder](http://www.phy.duke.edu/~rgb/General/dieharder.php)，成功地通过了所有的随机性测试。一个有趣的构建展示了生成真正的随机数有多难。