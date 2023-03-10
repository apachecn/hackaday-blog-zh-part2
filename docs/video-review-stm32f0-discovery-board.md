# 视频回顾:STM 32 f 0-发现板

> 原文：<https://hackaday.com/2012/05/30/video-review-stm32f0-discovery-board/>

[https://www.youtube.com/embed/H1KzDv7N3H8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/H1KzDv7N3H8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

STM32 发现板并不新鲜，我们已经看过几次了。但是这条线中最新的兄弟姐妹可能正是从你坚定的 8 位项目中跳跃出来的东西。我们得到了它，并记录了视频审查。

STM32F0-Discovery 将编程器和 ARM Cortex-M0 芯片集成在一块方便的电路板上。顶部是 ST-Link V2 编程器，包括跳线和一个编程头，可轻松对板外芯片进行编程。

内置的微控制器是 STM32F051R8T6，包括 64kb 程序存储器和 8kb RAM。单个器件的报价为 1.80-3.77 美元，采用可手工焊接的 LQFP 封装，这让我们对未来的项目感到惊讶。它有一个带 6x PLL 的 8 MHz 内部振荡器，这意味着你可以在没有外部晶体的情况下以 48 MHz 运行(如果你不知道这是什么，请查看[【肯尼斯·芬尼根的】PLL 初级读本](http://hackaday.com/2012/02/15/intro-to-phase-locked-loops/))。

唯一阻碍我们的是开发环境。如果你在 Windows 上，ST 提供你需要的一切，但是我们想要一个 Linux 友好的解决方案。我们知道，由于这个项目，其他发现板已经在 Linux [下工作。这使用相同的圣链接 V2，所以它应该工作得很好。如果你想在首页看到自己的头像，看看](http://hackaday.com/2011/10/17/how-to-develop-for-stm32-discovery-boards-using-linux/)[他们是否还在分发样品](http://www.st.com/internet/evalboard/product/253215.jsp)。应该有一个标有“注册免费工具包”的按钮。