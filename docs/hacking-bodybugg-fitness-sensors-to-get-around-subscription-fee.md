# 黑客入侵 BodyBugg 健身传感器以规避订阅费

> 原文：<https://hackaday.com/2012/11/28/hacking-bodybugg-fitness-sensors-to-get-around-subscription-fee/>

![](img/5daaea8e0746fe558d3cb8d7780a6633.png "bodybugg")

这个臂带是一个传感器包，当你戴着它的时候它会记录数据。它记录加速度计数据、皮肤温度和皮肤电反应。然后可以对这些数据进行分析，得出燃烧的卡路里等数据。但是…该设备背后的公司似乎已经包括了一种保持现金流的方法。一旦你买了它，你可以使用他们提供的 Java 程序从设备上读取数据。但是你不能删除设备上的数据，除非你订阅了他们的在线服务。一旦填满，就没用了。[Doug]对这个问题不满意，所以[他对清除 BodyBugg 内存的技术进行了逆向工程](http://www.bemasher.net/archives/1130)。

之前曾有过几次对该设备进行逆向工程的尝试，但那些基础工作并没有真正帮助到[道格]的探索。他最终从原始程序中反汇编了 Java 类。这帮助他想出了如何初始化通信。一旦到了那里，他很高兴地发现这个装置会告诉你如何使用它。如果你发出一个无效的命令，它会给出一个包含所有有效命令的列表。启动和运行所需的一切都可以在[他的 github repo](https://github.com/bemasher/BodyBuggBypass) 中找到。