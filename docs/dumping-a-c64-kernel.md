# 转储 C64 内核

> 原文：<https://hackaday.com/2012/09/14/dumping-a-c64-kernel/>

![](img/76c747f84fbc74794fb34fc40420b91d.png "c64-kernel-dumper")

[Blark]在 Craig 的清单上选了几台 Commodore 64 机器，这样他就可以在里面玩 SID 芯片了。但是那里有一些其他有趣的东西，他的注意力被存储内核的 PROM 吸引了。他认为建造一个能够存储二进制图像的 ROM 转储器会是一次有趣的冒险。

在休息后的视频中，您可以看到，当启动时，转储器立即开始向终端传输十六进制值。该系统被设置为输入 Python 脚本，该脚本将数据流打包成图像文件。读取由 PIC 18F4520 完成，以 9600 波特的速率流入数据，每个地址读取之间有很大的延迟，以获得尽可能清晰的读取。他从 AVR 怪胎那里得到了一点帮助。

我们猜测他会多次提取芯片上的图像，并比较结果，以过滤掉任何可能的数据损坏。从那以后，我们不确定他会用这些文件做什么，但是总是有可能用这个内核映像制作自己的模拟器。

[https://www.youtube.com/embed/nxjv6UuQUdE?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/nxjv6UuQUdE?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)