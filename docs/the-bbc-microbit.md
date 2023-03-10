# 微:bit — BBC 让百万儿童投入嵌入式开发

> 原文：<https://hackaday.com/2015/07/07/the-bbc-microbit/>

20 世纪 80 年代初，BBC 启动了一个项目，向一代英国小学生教授计算机知识。这个项目产生了 BBC Micro，一台非常强大的家用电脑，向一代人展示了电脑到底能做什么。这些孩子然后回家，打开他们的 ZX 光谱，成为一代软件工程师。尽管如此，英国广播公司的微型是深情地记住。

计算机革命早已结束，但今天我们遭遇了嵌入式处理器和微控制器的巨变。随着 Arduinos 和 Raspberry Pis 的推出，BBC 决定是时候将 ARM 微控制器的强大功能交到 100 万 11 岁和 12 岁的孩子手中了。[结果是微:位](http://www.bbc.co.uk/programmes/articles/4hVG2Br1W1LKCmw8nSm9WnQ/introducing-the-bbc-micro-bit)。这是一个小型微控制器板，带有 ARM 处理器、IMU、按钮、蓝牙和 5×5 LED 阵列——如果你正在教一百万个孩子如何闪烁 LED，这正是你需要的。

虽然 BBC [已经完成了微型钻头的设计](http://www.bbc.co.uk/mediacentre/mediapacks/microbit),*还没有任何规格。然而，可以做出一些有根据的猜测。USB 控制器由 Freescale 提供，该公司还提供数字罗盘和磁力计。编程是通过一个基于 web 的、类似 Arduino 的 IDE 来完成的，这个 IDE 看起来是一个不错的微比特专用库。该板还兼容 mbed。蓝牙，显然是 ARM Cortex M0 核心，是由一个北欧 nRF51822 提供的。只有三个鳄鱼夹兼容的 I/o，它怀疑任何学生将建立任何太复杂的入门级 ARM。也是 3V 逻辑；终于，5V 的暴政倒下了。*

Micro:bit 最好被视为一种工具，它使英国学校最近增加了一门计算机科学课程。现在有一个要求，要求七岁的孩子理解算法并编写简单的程序。以前，英国的计算机教育包括 PowerPoint。[现在，中学生将学习布尔逻辑](http://www.telegraph.co.uk/technology/news/10410036/Teaching-our-children-to-code-a-quiet-revolution.html)。

虽然微型钻头作为做实际工作的工具毫无用处，但教育不是真正的工作。对于闪烁几个 led，让设备对移动做出反应，玩蓝牙，以及其他电子产品的小缺点，Micro:bit 是很棒的。不是每个人都会成为这项倡议试图创造的数字技术专家，但对于那些倾向于分号和电子的人来说，这是一个很好的技术介绍。