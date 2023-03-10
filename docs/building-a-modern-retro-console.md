# 构建现代复古控制台

> 原文：<https://hackaday.com/2015/02/01/building-a-modern-retro-console/>

有几十个经典游戏机的经典重制版本，使用从 Uzebox 的 ATMegas 到每个人都喜欢的硬件，在 Raspi 上填充一些 rom，然后就结束了。你不需要*学习*任何这样做的东西，这使得【迈克】的[定制游戏控制台](http://infiniteprojects.blogspot.com.au/2015/02/a-new-game-console-project-part-4.html?m=1)远远超过其他的。

[构建从](http://infiniteprojects.blogspot.com.au/2015/01/a-new-game-console-project-part-1.html?m=1)开始，是一个带有双 ATMega GPU 的 Z80 计算机的计划。他在设计方面取得了足够的进步，这将是一个杰作，但无法在家里磨双面板扼杀了设计。然后计划转移到 FPGA，再转移到带有 ADI 公司 PAL/NTSC 编码器芯片 AD725 的 ATMega。这个想法和[的 Uzebox](http://belogic.com/uzebox/index.asp) 有相似的架构，但是【迈克】想要更大的功率。他最终选定了一款配有 AD725 的[pic 32。](http://infiniteprojects.blogspot.com.au/2015/01/a-new-game-console-project-part-2.html?m=1)

这种设置能够输出一些令人印象深刻的图形，但要将位移动到屏幕上，你需要 DMA。[Mike]遇到了一个问题，DMA 计时器以 3.7 MHz 的最大速率运行。这是几个项目中记录的问题，导致【迈克】再次改变计划，[这次是 STM32F4](http://infiniteprojects.blogspot.com.au/2015/02/a-new-game-console-project-part-4.html?m=1) 。

错误被解决了，现在[迈克]可以在屏幕上传输大量像素，同时仍有一些剩余的处理能力来玩游戏。这是一个已经超过一年半的项目，到目前为止他已经学到了很多。