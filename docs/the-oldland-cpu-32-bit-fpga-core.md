# Oldland CPU 32 位 FPGA 内核

> 原文：<https://hackaday.com/2015/03/20/the-oldland-cpu-32-bit-fpga-core/>

现场可编程门阵列(FPGAs)让你可以将任何你想要的逻辑编程到一个芯片上。您使用硬件描述语言编写逻辑，然后将其闪存到 FPGA。你甚至可以设计自己的处理器，并将其闪存到芯片中。

这正是[jamieiles]对[old land CPU](http://jamieiles.github.io/oldland-cpu/)所做的。这是一个开源的 32 位 CPU 内核，可以在 FPGA 上使用。你不仅可以浏览 [Github repo](https://github.com/jamieiles/oldland-cpu) 中的所有 Verilog 代码，还可以使用一堆工具来处理这个 CPU 内核。

软件包中包括 oldland-rtlsim，它允许您在 PC 上模拟处理器。oldland-debug 工具允许您通过 JTAG 连接到处理器进行编程和调试。最后，还有一个 GNU 工具链端口，可以让你为设备构建 C 代码。

更进一步，[jamieiles]在 Oldland core 周围建立了一个完整的 SoC。它具有 SPI、UART、定时器和更多微控制器应有的特性。可以闪到相对便宜的 Terasic [DE0-Nano](http://www.terasic.com.tw/cgi-bin/page/archive.pl?No=593) 板上。

[jamieiles]还将 u-boot 移植到了处理器上，接下来就是 Linux 内核了。如果你曾经对 CPU 的实际工作方式感兴趣，这是一个很好的项目。如果你想要更多的开源 CPU 内核，请查看 [OpenCores](http://opencores.org/) 。