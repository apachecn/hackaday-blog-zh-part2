# Fubarino 竞赛:串行数据传输

> 原文：<https://hackaday.com/2013/12/28/fubarino-contest-serial-data-transmission/>

![fubarino-contest-serial-data](img/461f35fd82a9adb7cb5fa47e27d31ac1.png)

[耶稣]正在帮助他的表弟学习微控制器。现在他们正在讨论串行通信的主题，这变成了添加一个 Hackaday 复活节彩蛋的好方法。

使用 FTDI 芯片和 PIC 18F4550(对他们来说直接实现 USB 还为时过早)串行数据显示在终端窗口中。同时，每个字节的二进制值在 PORTD LEDs 上闪烁。当芯片接收到字符“hack”时，它会立即[回显推荐，以检查 Hackaday](http://www.youtube.com/watch?v=ffQ7zofYdpk) 的牛逼之处。他将本例中使用的代码[作为要点](https://gist.github.com/JeshuaSan/8016026#file-pic18_usart_had_contest-c)。

* * *

这是 Fubarino 竞赛的参赛作品，有机会获得微芯片作为奖品提供的 20 块 [Fubarino SD 板中的一块。](http://www.microchip.com/stellent/idcplg?IdcService=SS_GET_PAGE&nodeId=1406&dDocName=en566210)

[https://www.youtube.com/embed/ffQ7zofYdpk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/ffQ7zofYdpk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)