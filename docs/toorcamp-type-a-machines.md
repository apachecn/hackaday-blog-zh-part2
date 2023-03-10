# toor camp:A 型机器

> 原文：<https://hackaday.com/2012/08/16/toorcamp-type-a-machines/>

[![](img/dc363356ffedd758b5dbde9e0f8f0747.png "Series 1")](http://hackaday.com/2012/08/16/toorcamp-type-a-machines/7773280724_a14376fd87_k/)

[Type A Machines](http://typeamachines.com/ "Type A Machines") 在旧金山设计和制造 3D 打印机。创始人之一的[Miloh]将他们的两款旗舰系列 1 打印机带到了 Toorcamp。他打印出了各种模型，包括防水杯和四轴飞行器臂。

[RepRap Arduino MEGA Pololu Shield](http://reprap.org/wiki/Arduino_Mega_Pololu_Shield "RAMPS")(斜坡)用于驱动每个轴的步进电机以及挤压机。这是附在运行[马林](https://github.com/ErikZalm/Marlin/ "Marlin") RepRap 固件的 Arduino MEGA 上的。Type A Machines 为打印机配备了可生物降解的[聚乳酸](http://en.wikipedia.org/wiki/Polylactic_acid "Polylactic Acid") (PLA)细丝。

在软件方面，你从 STL 格式的 3D 模型开始。这可以从 Google SketchUp 或 Autodesk 123D 等 3D 软件中导出。然后，您需要一个切片器来生成 g 代码和机器控制软件来命令打印机。[Miloh]在他的工作流程中使用了 [Slic3r](http://slic3r.org/ "Slic3r") 和 [Repetier](http://reprap.org/wiki/Repetier-Host "Repetier") ，但他也指出了 [3D 打印机工作流程](http://techwall.net/ultimaker-3d-printing-workflow "3D Printing Workflow")的一个很好的总结。

系列 1 于今年 5 月在湾区制造商博览会上推出。它的打印量为 1200 毫升，是所有台式打印机中打印量最大的。Series 1 为低成本 3D 打印机市场带来了另一种选择。