# 用 3D 打印机制作柔性印刷电路板

> 原文：<https://hackaday.com/2014/10/28/make-flexible-pcbs-with-your-3d-printer/>

在过去的几年里，廉价印刷电路板制造取得了长足的进步。如今，你可以在一周内制造出每平方英寸仅几美元的木板。尽管如此，柔性印刷电路板仍然相当昂贵。[Mikey77]正在改变这种状况，他用 3D 打印机在家里制作柔性电路。[Mikey77]利用了 Ninjaflex 热塑性弹性体(TPE)细丝的一种特性——它可以粘在裸铜上！

TPE 细丝充当抗蚀剂，类似于使用激光打印机墨粉的方法。对于基底，[Mikey77]列出了 3 个选项:

来自 Electronics Goldmine 的 [.004”厚的“剪刀切割”覆铜板](http://www.goldmine-elec-products.com/products.asp?dept=1034)

。 [002″厚纯铜涤塔夫面料](http://www.lessemf.com/fabric.html)来自 lessEMF.com

[< .001″ Pyralux 材料](http://www.adafruit.com/products/1894)来自 Adafruit，是用于制作专业柔性 PCB 的材料之一。

一点喷胶会把柔性印刷电路板固定在打印机的底座上。唯一的问题是说服打印机打印比实际床高千分之几英寸。[Mikey77]没有改变 Z 轴上的原点位置，而是使用 [AutoDesk 123D](http://www.123dapp.com/) 来创建 3D PCB 设计。他的每一个。stl 文件有一个“间隔条”，它位于床层。要打印的实际轨迹在床上方千分之几英寸的空中，正好是基底材料的厚度。打印机在底座上打印间隔条，然后提升其 Z 高度并在柔性 PCB 材料上打印。我们确信像这样强迫打印机在半空中打印会导致一些打印机软件抛出错误，但这个系统对[Mikey77]和他的 Makerbot 有效。

一旦设计印刷完成，电路板就用氯化铁等标准蚀刻溶液进行蚀刻。不过要小心——这些薄基板的蚀刻速度比普通 PCB 快得多。