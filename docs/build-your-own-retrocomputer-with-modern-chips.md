# 用现代芯片建造你自己的逆向计算机

> 原文：<https://hackaday.com/2014/09/16/build-your-own-retrocomputer-with-modern-chips/>

如果你曾经想开始逆向计算，或者你从 80 年代开始使用的 Commodore 64 刚刚放弃了幽灵，[Rick]又名[Mindrobots]正好适合你:基于 PIC 微控制器和视差推进器的[逆向计算机。](http://www.instructables.com/id/Building-your-own-Micromite-Companion-Minicomputer/step3/The-Micromite/)

计算机核心的两个芯片都是开源的。Propeller 是处理 I/O、视频和音频输出的完美主板，因为它是专为多任务机器而设计的。微控制器是 PIC32MX150 或 PIC32MX170，装载有一个基本解释器、19 个 I/O 引脚、一个全屏编辑器和许多通信协议。简而言之，复古风格的小型机应有尽有。

整个计算机可以组装在一个 PCB 上，具有你能想象到的所有输出(VGA、PS/2 等)，一旦完成，可以编程运行任何能想象到的程序，包括游戏。当然，它可以通过所有 I/O 连接任何物理设备，因为它的核心是一个微控制器。

逆向计算对于黑客来说是一个相当活跃的舞台，有些是由 FPGAs 制成的，而其他的准系统计算机是由 T2 的三个芯片制成的。很高兴在阵容中看到另一个伟大的计算机，特别是使用像 Propeller 和 PIC 这样的开放芯片的计算机。