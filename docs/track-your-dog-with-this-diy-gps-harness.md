# 跟踪你的狗与这个 DIY 全球定位系统线束

> 原文：<https://hackaday.com/2014/06/07/track-your-dog-with-this-diy-gps-harness/>

![GPS-dog-harness](img/295d6a86b75effb5c511f0b691c8f745.png)

你有没有想过，当你带你的狗去公园的时候，它实际上跑了多远？你可以是一个标准的消费者，花 100 美元或更多买一个 GPS 追踪项圈，或者你可以跟随[Becky Stern]的领导，建立你自己的简单而有效的 [GPS 追踪装置](https://learn.adafruit.com/gps-logging-dog-harness/ "GPS tracking harness")。

[Becky]在这个项目中使用了两个植物群模块；FLORA 主板和 FLORA GPS 模块。FLORA 主板本质上是一个小的、可缝合的 Arduino 板。GPS 模块显然提供了跟踪功能，但也有内置的数据记录功能。这意味着[Becky]不需要增加任何特殊记录电路的复杂性。GPS 坐标是以原始格式记录的，但可以很容易地粘贴到谷歌地图上查看，正如[Becky]在休息后的视频中演示的那样。该系统使用 FLORA 主板上的内置 LED 来通知用户 GPS 何时收到锁定以及程序是否正在运行。

整个系统依靠三节 AAA 电池运行，根据[Becky]的说法，这可以提供几个小时的跟踪。她还为 GPS 模块安装了一个小型硬币电池。这为 GPS 模块提供了备用电源，因此它可以记住其先前的位置。这不是必须的，但是它提供了一个好处，即 GPS 模块可以记住它最近的位置，因此可以更快地发现它的位置。

[https://www.youtube.com/embed/ID9dJE75VQU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/ID9dJE75VQU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)