# 通过三个简单的步骤(不那么简单)构建一个 FPGA 微型 bee

> 原文：<https://hackaday.com/2013/10/12/build-an-fpga-microbee-in-three-not-so-easy-steps/>

![Microbee,_Melbourne_Museum](img/2f471d0413fa04668ef297e118734b39.png)

[布拉德·罗宾逊]有点怀念他的微型手机，所以[他用 FPGA](http://fpgabee.toptensoftware.com/)重建了它。不是一次，而是三次。对于外行人来说，[应用技术微型计算机](http://en.wikipedia.org/wiki/MicroBee)是 1980 年代基于 Z80 的计算机。这种微型计算机在澳大利亚设计，在澳大利亚以外并不流行。即便如此，许多澳大利亚人对家用电脑的了解还是通过微型电脑实现的。[Brad]实际上为 Microbee 写了几个程序，包括应用技术公司自己卖的一些游戏。

快进到 2012 年，【Brad】正在学习 FPGAs，想用 VHDL 做一个 Microbee。FPGAbee 诞生了。FPGAbee 的第一次迭代是从 CPU 开始的，它来自于 [T80 开源 VHDL Z80 内核。](http://opencores.org/project,t80)围绕这一核心,【Brad】添加了视频控制器、键盘和声音。当他开始添加磁盘功能时，[Brad]遇到了一些问题。他想使用 FAT 格式的 SD 卡进行磁带和硬盘仿真。

FAT 格式相对复杂，这意味着他必须使用一些定制软件来完成这项工作。[Brad]决定在第二个 Z80 内核上运行该软件。两个内核都需要访问内存，这就是[Brad]在 FPGAs 上学习他所谓的“跨域时钟的艰难一课”的地方。多个时钟网络可能会导致严重的传播延迟问题。[Brad]能够解决这些问题，但这导致他后退一步，重新评估整个设计。这是 FPGABee2 的开始。

Brad 取消了双处理器设置，并重新设计了系统的一些其他部分。设计的第二次迭代顺利完成。在项目结束时，[Brad]在 Xilinx Spartan6 的数字 Nexys-3 板上仿真了一个 Microbee。虽然 Nexys-3 非常适合原型制作，但作为最终系统并不太实用。[Brad]不打算自己生产基于 BGA 的 PCB，所以他尝试了一种 [Xess Xula2 板](http://www.xess.com/shop/product/xula2-lx25/)。Xula2 确实需要一些移植工作，但[Brad]能够让系统启动并运行。一个定制的通孔 PCB 载板产生了一个光滑的成品项目，XulaBee。

[谢谢戴夫！]