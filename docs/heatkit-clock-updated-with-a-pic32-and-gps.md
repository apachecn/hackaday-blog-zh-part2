# 希斯基特时钟更新了 PIC32 和 GPS

> 原文：<https://hackaday.com/2013/11/01/heatkit-clock-updated-with-a-pic32-and-gps/>

![heathkit-clock](img/5bdb0e09810a1444e3ee5d4efb7e4b6c.png)

[鲍勃]最珍贵的财产之一是一个他小时候组装的希斯基特闹钟。这些年来，他注意到他的钟有一些问题。没有备用电池，所以停电时它会重置。设置时间和闹钟也是一件只能向前的事情——因此，为了夏令时，将时钟向后拨一小时意味着在时钟滚动 23 小时时按住按钮。[Bob]决定用一些现代部件改装他的时钟。虽然最简单的方法可能是拆掉时钟，但这不会保留所有经典的希斯基特部件。[Bob]所做的实质上是在系统中添加一个 PIC32 协处理器。

像 70 年代和 80 年代的许多时钟一样，希斯基特闹钟是基于国家半导体 MM5316 数字闹钟芯片。MM5316 在 8–22 伏下工作，因此它不能直接与 3.3V (5V 容差)PIC32 I/O 引脚接口。在 PIC 的输入端，[Bob]使用了几个模拟多路复用器芯片。PIC 可以扫描时钟显示的单个元素。在 PIC 的输出端，他使用了几个模拟开关来控制“快”、“慢”和“显示警报/时间”按钮。

PIC 现在可以读取和更改时钟的时间和闹钟。通过同时按下所有三个按钮，它可以重置到已知的午夜状态。唯一缺少的是实时数据源。[Bob]在系统中添加了 GPS 来完成这个任务。GPS 接收来自卫星的当前 GMT 时间，并将该数据发送到 PIC。然后，PIC 通过存储在 NVRAM 中的时区值对此进行补偿。报警时间也存储在 NVRAM 中。

开机时，PIC 首先设置时钟的闹钟。然后它等待 GPS 同步。一旦有了 GPS 时间，PIC 就会设置时钟。PIC 还会在每天午夜重置时钟时间。MM5316 仍然控制着一小时一小时的计时。这是一个伟大的黑客，是一个非常好的方式来添加功能到一个漂亮的 VFD 显示的经典时钟。

[https://www.youtube.com/embed/eRLdEsqccDc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/eRLdEsqccDc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)