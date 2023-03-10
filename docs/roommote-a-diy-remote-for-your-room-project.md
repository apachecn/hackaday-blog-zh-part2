# RoomMote，一款适合您房间项目的 DIY 遥控器

> 原文：<https://hackaday.com/2015/05/02/roommote-a-diy-remote-for-your-room-project/>

[Rohit]来信告诉我们他创造的一个项目。像大多数项目一样，他的解决了一个问题。有时睡觉时，一只蚊子会潜入他的房间。他有一个驱蚊器，但有两个问题，他必须起床来打开/关闭它，而且在使用时气味难闻。[Rohit]只需要一个遥控驱蚊器，但他决定制造一个 6 通道系统，他称之为 [RoomMote](http://rohitg.in/2015/05/01/RoomMote/) 。

从一开始，计划是使用一个旧的索尼电视遥控器来进行传输。接收器单元完全是从零开始制造的。[Rohit]围绕一个表面贴装 MSP430 芯片设计了自己的电路，并制作了一个非常好看的 PCB，以适应他的项目箱。MSP430 芯片被编程为基于从索尼遥控器接收的信号来打开和关闭继电器。这些继电器位于电气箱内，控制交流电源插座。只需将您的灯、收音机或驱蚊器插入适当的插座，即可进行无线控制。MSP430 的代码可以在[Rohit 的]项目页面上找到，任何人都可以制作类似的东西。

除继电器外，定制电路板上还附有一个 RGB LED 灯条。通过使用更多的索尼遥控器的按钮，LED 条可以输出 6 种预编程的颜色，为蚊子提供一些情绪照明！

[https://www.youtube.com/embed/hsQ9HEd14hQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&start=338&wmode=transparent](https://www.youtube.com/embed/hsQ9HEd14hQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&start=338&wmode=transparent)