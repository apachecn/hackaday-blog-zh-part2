# 从 SD 卡加载 Atari 游戏

> 原文：<https://hackaday.com/2013/06/12/loading-atari-games-from-an-sd-card/>

![Atari](img/75ee428180aba15181b6ebd96678525d.png)

它们不是 2600，但雅达利 400、800 和 1200 本身就是很棒的电脑。由于只读存储器中只有 BASIC 语言，它们不是特别有用或有趣，正如[耶鲁安]在购买一台带坏磁带机的 800 时发现的那样。有一些选项允许你从 PC 上加载仿真器文件，但是[耶鲁安]想要更紧凑的东西。他想出了一个用简单的微控制器从 SD 卡上下载游戏和应用程序的方法。

400、800 和 1200 都有一个端口，允许计算机与打印机、调制解调器、磁盘驱动器通信，并加载游戏。已经有一些电路将 SIO 端口连接到计算机，这样就可以加载游戏，但[耶鲁安]希望为他的 800 找到一个更紧凑、更便携的解决方案。

他想出的其实很简单。只有一个 Arduino，SD 卡和一个 LCD 显示器，允许他浏览 SD 卡上的目录并将其加载到 800 的内存中。

Atariage 论坛上的许多人都对[耶鲁安]的工作印象深刻，并希望自己也能得到一块这样的板。这个项目还没有完成——[耶鲁安]仍然需要为他的设备做一个案例——但希望他能在未来几个月里旋转几块板子。

你可以在下面看到这款设备的两个视频。

[https://www.youtube.com/embed/zl2DFLIxzV0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/zl2DFLIxzV0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)
[https://www.youtube.com/embed/0SZ8zClsYu4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/0SZ8zClsYu4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)