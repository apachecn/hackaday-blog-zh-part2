# Papilio Duo: FPGA、逻辑分析仪、调试器和 Arduino 兼容

> 原文：<https://hackaday.com/2014/05/29/papilio-duo-fpga-logic-analyzer-debugger-and-arduino-compatible/>

![Back](img/5e3389891a646f777b67b3c4fbdfb407.png)

我们已经有一段时间没有看到一些结合 FPGA 和 Arduino 的新主板了，所以技术水平自然有点落后。杰克·加塞特(Jack Gassett)的最新作品[Papilio Duo](https://www.kickstarter.com/projects/13588168/papilio-duo-drag-and-drop-fpga-circuit-lab-for-mak)旨在改变这种情况，解决最初 Papilio 的所有抱怨，并添加一些你会在 2014 年设计的电路板上看到的简洁、现代的功能。

这两个器件上有一个 ATMega32u4，与 Arduino Leonardo 中使用的芯片相同，可以轻松与标准 Arduino 项目集成。棋盘的顶部是真正的钱所在。有一个具有 9k 逻辑单元的 Spartan 6 FPGA，足以运行模拟昔日的一些经典计算机，包括著名的 SID 芯片雅马哈 YM2149 和 Atari POKEY(！).有了主机和设备 USB、SRAM 的 512k 或 2M 以及 FPGA 输入上的 ADC，该板应该能够处理您想要的一切。在底部甚至有一个 HDMI 的突破。

这对组合有一些有趣的软件功能，包括一个用于 ATMega 芯片的完整调试器，这要归功于一个仿真的 Atmel JTAG ICE MKII。是的，兼容 Arduino 的主板终于有了一个真正的调试器。FPGA 还可以实现一个 32 通道逻辑分析仪，这不仅是一个非常强大的开发板，也是一个有用的工具。