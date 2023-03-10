# 8x8x8 LED 立方体和驱动它的电路板

> 原文：<https://hackaday.com/2012/11/22/8x8x8-led-cube-and-the-board-that-drives-it/>

看看他带领[托马斯]、[马克斯]和[菲利克斯]组成的立方体。但是不要忘了看看驱动它的漂亮 PCB 太棒了！但是硬件只是像这样一个项目的一部分。烙铁冷却后，他们继续工作，编写自己的软件来生成三维显示的图案。

看着这样一个干净的构建，并不能让你明白要让一切正常运行，你需要建立多少连接。要欣赏它，你应该看一看[另一个 512 LED 立方体](http://hackaday.com/2011/03/18/512-led-cube-again/)，它有电线显示。你可以从原理图中看到(可在[项目库](https://github.com/xythobuz/LED-Cube)中获得)，所有这些线路都由一系列移位寄存器管理。该板本身连接到一台计算机，从该计算机获得可视化命令。他们称之为 CubeControl 的 Java 程序可以推送字母或将立方体变成 VU 计。

该团队至少建造了其中的两个。这个较小的版本使用红色 led，而在休息后的视频中显示的较大的版本使用蓝色 led。

[https://www.youtube.com/embed/czxCxTBSgHM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/czxCxTBSgHM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)