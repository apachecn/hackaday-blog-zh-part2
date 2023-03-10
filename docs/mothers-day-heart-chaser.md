# 母亲节追心者

> 原文：<https://hackaday.com/2012/05/16/mothers-day-heart-chaser/>

![](img/bd08e5dc6243fea354d2de8bd9d66582.png "mothers-day-heart-chaser")

[罗伯特·米布斯]接手了一个项目，他的孩子可以在母亲节送给妈妈。这是一个嵌入戒指或项链盒的 LED 心形图案。这一系列白色发光二极管以追逐模式显示动画。这个项目让[罗伯特]突破了舒适的界限，超越了 Arduino 主板。

在里面你会找到一辆 ATtiny85。他拿起芯片尝试在更小的硬件上运行 Arduino 草图。但是总共五个可用的 I/O 引脚在驱动 led 时出现了问题。这里使用了十个发光二极管，即使是标准的多路显示器也需要不少于七个来控制它们，而不需要额外的芯片，也不需要 [Charlieplexing](http://hackaday.com/2012/05/03/an-attiny13-makes-may-13th-brighter/) 。他的解决方案是同时驱动两个相反的 led，这就减少了对五个可用引脚的需求。

一旦他把所有的东西焊接在一起，他意识到他犯了一个编码错误。但是一些焊接的电线让他可以用 ISP 重新安装。

[https://www.youtube.com/embed/YXHQr8U3EQI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/YXHQr8U3EQI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)