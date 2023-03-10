# 高压水下机器人冒险

> 原文：<https://hackaday.com/2012/08/20/high-voltage-rov-adventures/>

![](img/b2d03089b102c1fa824b0d2f8407e329.png "high-voltage-rov-adventures")

[Eirik]写来分享他的水下 ROV 第三次迭代的建造日志。前两个项目已经完成并经过测试(你可能还记得[在一月份读到的](http://hackaday.com/2011/01/15/two-generations-of-ocean-going-rov/)，但是两个项目都有导致普遍失败的问题。最值得注意的是，在他不想要的地方引入水。但这一次，他似乎一切都做对了，成功地将这个小家伙带到了 20 米深的地方，没有一点泄漏。

他在第二版中遇到的一个问题是从地表供电。他需要 12V 高达 10A 的电压，必须使用 14 AWG 的系绳才能实现。这需要拖着很多沉重的电线，这使得 ROV 实际上无法移动自己。他想回到使用 Cat5e 电缆，但它不能处理这种电流。他最终在水面使用逆变器将电压升至 130V，并在 ROV 上使用开关模式电源将电压恢复至 12V。这导致了数据线上的噪声，他通过在逆变器的输出端增加一个全波整流器来解决这个问题。

休息后的潜水视频展示了这个东西可以捕捉到的清晰的镜头。

[http://www.youtube.com/watch?v=2QBmg7LVZgQ](http://www.youtube.com/watch?v=2QBmg7LVZgQ)