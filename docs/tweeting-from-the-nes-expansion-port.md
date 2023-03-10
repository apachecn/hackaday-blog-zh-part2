# 从 NES 扩展端口发推文

> 原文：<https://hackaday.com/2015/05/01/tweeting-from-the-nes-expansion-port/>

[Trapper]是一个 80 年代的孩子，当年任天堂娱乐系统是他的最爱。在一个决定命运的夜晚，他把他最喜欢的灰色盒子翻了过来，取下一个小塑料保护罩，露出了神秘的扩展端口。这是为了什么？任天堂会用它做什么？

NES 上的扩展端口并没有真正用于任何事情，至少在美国市场是这样。即使在自制软件领域，也只有一个搁置的项目允许 NES 连接外部设备。为了实现[陷阱]童年的梦想，他必须为 NES 扩展港建造一些东西。Twitter 似乎是一个不错的应用。

创建 NES 扩展端口 Twitter 的第一步是探测这个连接器的深度。CPU 的整个数据总线都在那里，还有一些盒式磁带通过引脚和一条地址线。该系统的设计使用了一个微控制器和一小块与 NES 共享的 SRAM。这个 SRAM 在微控制器和 NES 之间共享消息，告诉 uC 发布消息，或者告诉 NES 在屏幕上显示消息。

扩展端口上只有一个地址引脚——A15——可用，但[Trapper]需要读写内存的某个部分，起价 6000 美元。这意味着地址 A13 和 A14 也需要被访问。幸运的是，盒式磁带插槽上有这些引脚，扩展连接器上有许多盒式磁带直通引脚。在未使用的墨盒的几个引脚之间做一个桥解决了这个问题。

从那里，它只是一个微控制器和 NES 之间的一系列信息传递。在[Trap]的兄弟[Jered]和服务器上运行的 Twitter 中继应用程序的帮助下，这个 NES 实际上可以发推特了。你可以在下面看到一段视频。

[https://www.youtube.com/embed/S38jQMs5wAk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&start=27&wmode=transparent](https://www.youtube.com/embed/S38jQMs5wAk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&start=27&wmode=transparent)