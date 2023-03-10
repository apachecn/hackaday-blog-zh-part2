# 用非常非常小的 IC 制作原型

> 原文：<https://hackaday.com/2012/08/17/prototyping-with-very-very-small-ics/>

[![](img/0dad855c4766e8d330426923870e5bcf.png "IC")](http://hackaday.com/wp-content/uploads/2012/08/ic.jpg)

一去不复返的日子，所有的酷芯片能够扔进一个试验板非常容易。[starlino]正在研究一种使用加速度计的电路，但不幸的是，这些芯片很难焊接 LGA-16 封装。[starlino] [想出了一种用这些封装制作原型的方法](http://www.starlino.com/reverse_surface_mount.html)，这种方法不需要定制分线板，也不需要花时间观察回流炉。

[斯塔里诺]的 LGA-16 适配器板从一块 perf 板钻出来形成一个完全适合他的加速度计的空间开始。将一片胶带放在芯片和 perf 板的焊盘上，芯片和板之间的间隙用两部分管道油灰填充。

一旦油灰固化，用[银导电笔](http://store.caig.com/s.nl/sc.2/category.174/.f)将加速度计上的导线连接到电路板上的衬垫上。在电路板的角落里放了几个插头引脚后，[starlino]将焊盘焊接到引脚上，为一个非常小的加速度计提供了一个永久的分线板。

这绝不是一个漂亮的建筑，但在[starlino]将整个建筑密封在液体电工胶带中并将其安装在 DIP 插座中后，他在一个易于原型化的封装中拥有了一个完全功能性的加速度计。对于一个可以用放在工作台上的材料搭建的分线板来说，这已经不错了。