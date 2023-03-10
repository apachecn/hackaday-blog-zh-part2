# 逆向工程一个游戏男孩克隆的启动 ROM

> 原文：<https://hackaday.com/2014/12/11/reverse-engineering-a-game-boy-clones-boot-rom/>

[nitro2k01]得到了一个游戏斗士，一个原版游戏少年的克隆体。虽然有大量关于原版 Game Boy 的引导 ROM 和操作的信息，但对这些克隆体却知之甚少。[nitro2k01]想要了解更多，所以他使用了一种[时钟故障技术来转储设备的 ROM](http://blog.gg8.se/wordpress/2014/12/09/dumping-the-boot-rom-of-the-gameboy-clone-game-fighter/) ，并在此过程中发现了一些关于其版权保护和引导过程的有趣发现。

看 Game Boy ROM 的内容有点挑战性。ROM 在引导时是可读的，但是之后 ROM 的地址空间被重新映射用于中断向量和其他用途。有两种方法可以解决这个问题，但最简单的方法是将晶体的一根引线接地。这导致 CPU 跳转到内存中的随机位置。最终 CPU 会跳到一个可以访问引导 ROM 的位置(如果你幸运的话！).

虽然[nitro2k01]的克隆可以运行与 Game Boy 相同的游戏，但它有不同的启动 ROM，也有一些显著的硬件差异。[nitro2k01]设法使用水晶接地技术的改良版本来干扰他的时钟并转储克隆人的启动 ROM。他发现克隆人使用了 Game Boy 版权检查技术的一种不寻常的变体，以及其他一些奇怪的东西。【nitro2k01】还贴了一张 boot ROM 的拆解，他解释的很详细。

谢谢你的提示。