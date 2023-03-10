# 温度数据记录器记录一段时间内的温度

> 原文：<https://hackaday.com/2015/01/09/temperature-data-logger-logs-temperature-over-time/>

![Temperature Data Logger](img/60923e9de0f0d77f1f40f58e8344360b.png)“胡珊”不仅喜欢他的电子项目，而且显然也喜欢记录它们。他在自己制作的[温度数据记录器](http://www.instructables.com/id/Temperature-Data-Logger-1/)上写了一个很好的指令，谢天谢地，他的代码可供他人使用。最终产品设计简洁，适用于防风雨的户外应用。

正如你所料，这个操作背后的大脑是一个 Arduino。它与一个实时时钟和一个 SD 卡模块相连，前者用于保持精确计时，后者用于存储收集的数据。在这种情况下，温度由 LM35 温度传感器读取，该值与时间一起以一分钟为间隔记录到 SD 卡上的. csv 文件中。

还有一个液晶显示屏，显示日期、时间和当前温度。为了节省电池寿命，LCD 背光通常是关闭的。它可以使用与外壳顶部的霍尔效应传感器相互作用的磁铁来打开。这非常有效，以至于[胡沙姆]在外壳的侧面安装了第二个霍尔效应传感器，用于重置 Arduino。说到箱子，它是一个防风雨的 PVC 电箱，底部安装了导管适配器。由两个旧笔记本电池组成的电池组装在一根导管中，为 Arduino 和其他组件提供 7.2 伏电压。不幸的是，没有关于电池组持续多长时间的消息。一旦记录了数据，就可以取出 SD 卡。在电子表格软件中打开 csv 文件，以制作显示温度随时间变化的图表。