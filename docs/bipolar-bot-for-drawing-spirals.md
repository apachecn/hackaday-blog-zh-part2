# 用于绘制螺旋的双极机器人

> 原文：<https://hackaday.com/2015/01/23/bipolar-bot-for-drawing-spirals/>

[Bart Dring]因 buildlog.net 激光切割机 Makerslide 以及与 Carvey 数控机床 Inventables 的合作而闻名于世。它们都是受欢迎的项目，都非常有用。这个就不太好了。这是一个不太把自己当回事的双极机器人，今年的构建为【Bart】通常用于 ORD Camp 的 gonzo 数控机器。

双极机器人——是的，这就是它的名字——很像一个 SCARA 机器人。在两臂的连接处有两个 NEMA 14 步进器，每个步进器都用螺栓固定在底板上的轴承上，另一端握着一支笔。就机械结构而言就是这样，但是软件非常有趣。

步进器由 Arduino 在一个工具的帮助下驱动，该工具将笛卡尔 Gcode 转换为机器所需的双极 Gcode。这涉及到一些数学问题，但是如果你能编写一些 trig 函数，就没什么值得注意的了

现在这个双极机器人正忙着画一些看起来像是从肺活量描记器里出来的东西。你可以在下面看到一段视频。

[https://www.youtube.com/embed/YBTTDfgHi8c?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/YBTTDfgHi8c?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)