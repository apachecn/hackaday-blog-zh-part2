# 深入了解 NES 俄罗斯方块

> 原文：<https://hackaday.com/2014/01/28/a-deep-dive-into-nes-tetris/>

[![Tetris AI](img/2b63d1dc972ede5a339a53a476a4a10c.png)](http://hackaday.com/2014/01/28/a-deep-dive-into-nes-tetris/tetris-5/)

早在 1989 年，任天堂为 NES 发布了俄罗斯方块。这篇详细的文章首先解释了俄罗斯方块如何工作的[机制，然后构建了一个人工智能来玩游戏](http://meatfighter.com/nintendotetrisai/ "Applying Artificial Intelligence to Nintendo Tetris")。

为了理解游戏的机制，我们研究了 ROM 的源代码。由于 NES 是基于 [MOS 6502](http://en.wikipedia.org/wiki/MOS_Technology_6502 "MOS 6502 on Wikipedia") 微处理器，这涉及到查看 6502 组件。这篇文章详细介绍了块(称为 Tetriminos)是如何创建的，以及它们如何在屏幕上移动。检查用于随机数生成的[线性反馈移位寄存器](http://en.wikipedia.org/wiki/Linear_feedback_shift_register)。甚至法律屏幕和演示模式的细节都有解释。

在参观了俄罗斯方块的工作原理后，一个人工智能的算法被展示出来。这个 AI 是在 [FCEUX](http://www.fceux.com/ "FCEUX") NES/Famicom 仿真器内部的 Lua 中实现的。它的工作原理是评估所有可能放置每个新的四亚氨基的地方，并根据一系列标准选择最佳位置。通过使用[粒子群优化](http://en.wikipedia.org/wiki/Particle_swarm_optimization)来确定每个标准的权重。

本文提供了代码的 Lua 版本和 Java 版本的源代码。运行人工智能所需的一切都是免费的，除了俄罗斯方块 ROM。如果你对 8 位游戏是如何构建的感兴趣，这篇文章是一个很好的读物。

[via [Reddit](http://www.reddit.com/r/programming/comments/1waneg/mechanics_of_nintendo_tetris_6502_asm_and_how_to/)