# 将 NES 填充到 FPGA 中

> 原文：<https://hackaday.com/2013/01/23/stuffing-an-nes-into-an-fpga/>

![megaman_fpga](img/5f222f8d9f752a55fc7ce523d01a1893.png)

当 Torrent torrent 客户端和 ScummVM LucasArts 冒险游戏解释器的开发者感到无聊时，一定会发生一些很酷的事情。对我们来说幸运的是，[Ludde]在圣诞节期间有点无精打采，时间比精力多得多，[在 FPGA 开发板上实现了任天堂娱乐系统](http://fpganes.blogspot.se/2013/01/luddes-fpga-nes.html)。

NES 由理光 2A03 CPU 驱动，这种芯片与 20 世纪 80 年代初 Commodore 64s 和 Apple IIs 中的 6502 几乎相同。不过，两者之间还是有一些区别:NES CPU 在芯片上包括一个音频处理单元，并连接到 NES 上一个非常酷的图像处理单元。[Ludde]把所有这些芯片放在他的 Spartan-6 FPGA 里，里面有很多 Verilog 代码。

系统的其余部分 RAM、显示输出和控制器输入来自连接到 FPGA 开发板的外设。[Ludde]的特定板没有良好的数模转换器，因此复合输出被交换为 VGA 输出。这不是一个完全准确的调色板，但对于一个只是感到无聊的人来说，这仍然是一件了不起的作品。