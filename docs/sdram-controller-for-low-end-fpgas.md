# 面向低端 FPGAs 的 SDRAM 控制器

> 原文：<https://hackaday.com/2013/10/11/sdram-controller-for-low-end-fpgas/>

[![](img/10c4c4e59cbea82b95bb30e59bb3d567.png)](http://hackaday.com/wp-content/uploads/2013/10/mc_init.jpg)

很少有“最新”的 FPGAs 可以轻松焊接。由于 io 数量众多，它们通常采用球栅阵列(BGA)封装。Xilinx Spartan 6 LX9 是一款 TQFP144 FPGA(引脚间距为 0.5 毫米)，是可用于制造低端开发板的少数例外之一。然而，它没有太多的逻辑和内存资源，也没有在硅片中实现片上内存控制模块。因此，[Michael]为它设计了一个占地面积很小的 SDRAM 控制器。

从头开始编写 SDRAM 控制器不适合胆小的人——首先，你必须知道 SDRAM 是如何工作的(RAS、CAS、预充电、刷新周期),而且由于需要高速和精确的时序，你还必须了解 FPGA 片外接口的一些细节。此外，大多数公开可用的开放内核都非常复杂，例如，仅 opencores.org 上 sdr_ctrl 控制器的 RTL 内核就加起来超过 2700 行 Verilog。即使这不是一个准确的比较指标，[Michael]的控制器也只有 500 行长。