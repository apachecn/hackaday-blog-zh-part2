# CNC 路由器转换为 3D 打印机

> 原文：<https://hackaday.com/2014/10/07/cnc-router-converted-to-3d-printer/>

在过去的几年里，3D 打印机的价格已经大幅下降。如今，甚至有可能花 200-300 美元买到一套 3D 打印机。这些廉价打印机的性能如何尚有争议。[Jon]想要一台能够进行高质量打印的打印机，而不需要倾家荡产。在研究了可用的不同 RepRap 类型后，他得出结论，他真的不适合完整的机器构建。他之前已经建造了一台 CNC 路由器，并决定最好在已经建造好的 3 轴框架上[添加一个热端和挤压机](http://www.jonshobbies.com/convert-a-cnc-router-to-a-3d-printer.html)。

CNC 刳刨机框架由铝制成，非常坚硬，并且具有 2’乘 2’的切割区域。所有轴在 THK 线性轴承上平稳滑动，由壁虎 540 步进驱动器驱动的 NEMA 23 电机提供动力。刳刨机已从机器上拆下，但安装支架仍保留。然后修改支架以固定挤出机和热端。对于 3D 打印机，通常有一个控制板，专门设计用于控制热端温度的专用输出。由于[Jon]已经为路由器安装好了电子设备，他不需要专门的 3D 打印机控制板。他确实需要一种方法来控制热端的温度，他通过使用独立的 PID 做到了这一点。PID 是手动设置的，不向计算机或控制板提供反馈。

![Huge Whistle](img/052e7579915702240cbd5b8bffdc385a.png)【Jon】喜欢用 Mach3 来控制他的 CNC 路由器，所以他坚持用它来打印。他尝试了一些切片器，但似乎 Slic3r 最适合他的设置。g 代码生成后，通过 Mach3 运行，以控制机器。[Jon]承认，他有办法调整设置，并且由于机架和托架的质量，打印速度比大多数只打印的机器慢。即便如此，他巨大的哨子印看起来相当不错。休息后在视频中查看一下…

[https://www.youtube.com/embed/5V0L4fpNyfU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/5V0L4fpNyfU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)