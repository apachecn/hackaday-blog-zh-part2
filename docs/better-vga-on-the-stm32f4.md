# STM32F4 上更好的 VGA

> 原文：<https://hackaday.com/2015/06/07/better-vga-on-the-stm32f4/>

[Cliff]正在将 VGA 视频以 800×600 的分辨率和每秒 60 帧的速度推出微控制器。这个微控制器没有视频硬件。在我们进入技术概述之前，[这里有一个非常令人印象深刻的演示](https://www.youtube.com/watch?v=7yXxhvKmVb0)。

讨论中的微控制器是 STM32F4，这是一款相当强大的处理器，我们已经看到它在一些非常有趣的应用中有很多用途。我们之前在 STM32F4 上见过 800×600 的 VGA，有[一个圆圈和文本演示](http://hackaday.com/2015/01/04/800-x-600-vga-with-the-stm32f4/)和[位盒控制台](http://hackaday.com/2013/09/18/the-bitbox-console-an-open-source-gaming-rig/)。[克里夫]的建筑更有能力，虽然；他运行着 800×600 @ 60FPS，使用一个欠锁的 CPU，并且微控制器的大部分(90%)资源都是空闲的。

然而，这不仅仅是一个演示；[Cliff]正在撰写一份在该芯片上生成 VGA 的完整教程。它以[推动像素](http://cliffle.com/article/2015/06/06/pushing-pixels/)的介绍开始，很快他将有一个关于定时和他的光栅化框架的演练。

仅仅因为[Cliff]费尽周折将这些教程放在一起，并不意味着你不能拿出一个 STM 发现板，制作自己的微控制器视频黑客。[Cliff]有一个完整的图形库，允许其他人构建时髦的视频应用程序。