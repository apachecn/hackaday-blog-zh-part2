# 用 PIC 生成视频

> 原文：<https://hackaday.com/2015/01/05/generating-video-with-the-pic-16/>

[ bekeband]最近偶然发现一个老旧的工业显示器。它很小，单色，有漂亮的绿色荧光粉，不接受复合信号。相反，有一个奇怪的 TTL 输入，带有水平同步、垂直同步和视频连接器。被激起了兴趣，[bekeband]把它带回家，开始着手一个驱动这种显示器的项目。[他成功了，带着一个我们在黑客提示行上看不到的芯片](http://www.bekeband.hu/index.php/2-uncategorised/1-video-generator-with-pic):16 位 PIC。

该项目使用了 [dsPIC30F3011](http://www.microchip.com/wwwproducts/Devices.aspx?product=dsPIC30F3011) ，一个奇怪的 40 引脚封装的 16 位小 PIC。这个版本的电路板实际上来自早期版本，在将水平同步、垂直同步和视频连接到这个小电路板后，[bekeband]开始编写一些代码。

有两个为该板编写的程序。第一个是静态图像测试器，它在 CRT 上显示单个图像。第二个是一个[，显示一个简单的动画](https://github.com/bekeband/MonitorTesterMovie)，在这个例子中，一匹马在原地奔跑。这不是最奇特的项目，但它确实有效，尽管[贝克班德]没有使用高速手臂，但他从这个芯片中获得了相当高的分辨率。

下面视频。

[https://www.youtube.com/embed/brN4EVD0-BA?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/brN4EVD0-BA?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)