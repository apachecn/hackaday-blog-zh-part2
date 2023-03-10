# 清点游戏机里的晶体管

> 原文：<https://hackaday.com/2014/12/18/counting-transistors-in-the-playstation/>

在俄罗斯，有一些人正在进行非常深入的技术拆解，最近的一次是有史以来最雄心勃勃的一次。PSXDEV 团队正在[撕裂原始 PlayStation](http://psxdev.ru)([Google translatrix](https://translate.google.com/translate?sl=ru&tl=en&js=y&prev=_t&hl=en&ie=UTF-8&u=http%3A%2F%2Fpsxdev.ru%2F&edit-text=&act=url))的核心，查看 30 万个晶体管，并在逻辑级模拟器中重新实现整个控制台。

虽然 PSX 中的 CPU 是该特定硬件独有的，但在其他地方可以找到许多这种定制芯片。内核——RISC LSI lr 33300——记录在一些罕见的书籍中，这些书籍在互联网上可以免费获得。这个芯片的其他部分就有点陌生了。有一个奇怪的寄存器，一个处理各种设备和外设之间的访问的总线单元，以及一个电影解压缩器。

逆向工程过程从拆开 CPU、GPU、声音处理单元和 CD-ROM 控制器的封装开始，拍摄非常高放大率的芯片照片，并慢慢绘制出半导体和金属，以弄清楚什么细胞做什么功能，它们是如何连接的，以及整体情况是什么。这是一个艰苦的过程，需要梳理千兆字节的模具镜头，并用 MS Paint 突出显示大门、电线和总线。

眯着眼睛看显示器的最终结果是用 Logisim 把芯片的轨迹变成逻辑元素。从那里，可以理解、研究 CPU 的功能，是的，最终模拟到门级。这是一项惊人的事业，真的。

如果这种事情听起来很熟悉，你是对的:PSXDEV 背后的同一个团队也负责类似的专注于任天堂娱乐系统的工作。在那里，NES(理光 2A03)内部的 CPU 被拆下，露出 6502 内核、APU、DMA 和所有使其成为定制芯片的额外部件。

谢谢[Rasz]的提示。