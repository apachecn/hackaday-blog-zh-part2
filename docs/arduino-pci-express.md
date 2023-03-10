# Arduino (PCI) Express

> 原文：<https://hackaday.com/2015/07/24/arduino-pci-express/>

如今几乎不可能找到一台带有旧 ISA 卡插槽的个人电脑。全尺寸 PCI 卡插槽也面临着同样的危险。如今，许多电脑都配备了 PCI Express 连接器。PCI Express 提供了许多优势，包括尺寸小、引脚数少，以及点对点串行总线拓扑结构，允许不同端点对之间的多个同时传输。除了个人电脑，你还会在其他东西上发现 PC Express 连接器，包括许多更大的嵌入式系统。

如果你想在 PCI Express 上做原型，你通常会求助于 FPGA。然而，[moonpuncorg]在迷你 PCI Express 板上发布了一个可行的 Arduino 设计。(正如[imroy264]在评论中指出的，该板正在使用 PCI-E 连接器上的 USB 端口。)设计文件使用 KiCAD，因此复制或更改应该相当容易。自然，边缘上有引脚来访问 I/O 端口和电源。你确实需要使用 ISP 来编程芯片上的 Arduino 引导程序。

该板对主机来说就像 Pro Micro 3.3V 板一样有趣，从那里你可以轻松地使用 Arduino IDE 为带有 PCI Express 插槽的计算机添加功能。已知该板与 VIA VAB-600 跳板和 VIA VAB-820 板一起工作，尽管它也可能与其他 PCI Express 主机一起工作。