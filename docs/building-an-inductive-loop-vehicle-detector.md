# 构建感应线圈车辆检测器

> 原文：<https://hackaday.com/2014/04/04/building-an-inductive-loop-vehicle-detector/>

[![](img/fa6636a88518b792ecbe70a499df531e.png)](http://hackaday.com/wp-content/uploads/2014/04/c_843_img1.jpg)

[Trax]被一个朋友要求制作一个装置，它可以[检测到车库大门前的汽车](http://www.elektronika.ba/843/inductive-loop-vehicle-detector-v2-1/)的存在，让它自动打开。在网上搜索了这样一个项目并尝试了许多之后，他决定基于[感应回路](http://en.wikipedia.org/wiki/Induction_loop)建造自己的探测器。你可能已经猜到了，这种探测器的工作原理是检测埋在道路中的线圈的电感变化。让一辆车在它上面几英寸的地方通过，会产生这样的效果。

[Trax]的报道显示了一个非常好的想法和专业的设计。使用 DIP 开关和按钮可以调整所有检测机参数:检测类型(存在/脉冲)、信号过滤、主频率和灵敏度。使用 1:1 隔离变压器将线环与主传感器电子设备隔离，并使用[科尔皮兹振荡器](http://en.wikipedia.org/wiki/Colpitts_oscillator)来驱动后者。此外，气体放电管也用于防雷。

电感的变化转化为谐振频率的变化，该变化随后被主微控制器检测到。该板采用 24V 交流供电，二极管桥+ LM2596 SMPS 降压转换器负责以有效的方式产生所需的+5V 电压。

似乎这还不够，[Trax]还开发了一个基于 PC 的工具，可以使用串行连接更改其他平台的设置。所有的资源都可以从他的网站上下载，休息后会嵌入一些视频。

[https://www.youtube.com/embed/LGw8DLDoRyY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/LGw8DLDoRyY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/40VQaZ4XrIQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/40VQaZ4XrIQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)