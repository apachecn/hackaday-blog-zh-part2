# Commodore 1530 数据集的 VU 计指示器

> 原文：<https://hackaday.com/2015/04/11/a-vu-meter-indicator-for-a-commodore-1530-datasette/>

对于现在拥有老式 Commodore 计算机的人来说，保证数据和程序的安全和备份是头等大事。磁盘驱动器存储在美国更普遍，而在欧洲，盒式录音带是首选的存储介质。

Datasette 设备允许将盒式磁带连接到计算机。磁头对齐对于成功地向磁带读写数据至关重要。有些型号的 Datasette 在按键上方有一个小孔，可以通过它来调整磁头的方位位置。在看信号指示器的时候调整这个可以帮助你改善坏磁带的信号，防止装载错误。[Jani]尝试了一种叫做“Load-IT”的商业解决方案，它有一个 led 条形图，但它对处理信号非常差的磁带没有太大帮助。所以他为他的数据集造了一个[信号强度计。他称之为 VU-塞特，因为它使用了一种模拟式仪表，与许多音频设备中的 VU 仪表非常相似。](http://blog.worldofjani.com/?p=1127)

[硬件](http://blog.worldofjani.com/?p=1477)很简单，使用常见的可用部件。模拟仪表是从易贝的电池检查器中提取的。一个运算放大器驱动模拟仪表，另一个晶体管驱动单独的扬声器。如果通过按钮启用扬声器，这可用于收听磁带。[Jani]在订购原型板之前，首先对电路进行了试验和测试。

为了测试性能，[Jani]使用了 [FinalTAP](http://www.coder.pwp.blueyonder.co.uk/finaltap.htm) ，这是一种为 Commodore 64 计算机检查、清理和恢复数字化数据盒式磁带(TAP 文件)的工具。“LOAD-IT”版本适用于状况相当好的磁带。但他的 VU-塞特版本允许他更精确地调整磁头，从坏磁带中获得更好的读数。在这个问题上，看看这个漂亮的[1530](http://hackaday.com/2014/08/09/commodore-1530-datasette-gets-a-digital-counter/)的 7 段气泡 LED 数字计数器。

[https://www.youtube.com/embed/uF8RRqpGqsc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/uF8RRqpGqsc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)