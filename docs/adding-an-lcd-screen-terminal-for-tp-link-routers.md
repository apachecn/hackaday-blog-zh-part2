# 为 TP-Link 路由器添加 LCD 屏幕终端

> 原文：<https://hackaday.com/2013/01/07/adding-an-lcd-screen-terminal-for-tp-link-routers/>

运行嵌入式 Linux 的路由器提供了相当多的功能，这取决于你需要做什么。为了扩展 TP-Link 路由器的用途,[Roman]建造了一个装备，增加了一个 LCD 屏幕来显示终端。但它最终比那更强大。

项目的第一部分是为显示器制作一个 USB 视频卡。【罗曼】带了一个 [STM32 开发板，用 QVGA 屏幕驱动](http://habrahabr.ru/post/163689/) ( [译](http://translate.google.com/translate?hl=en&sl=auto&tl=en&u=http%3A%2F%2Fhabrahabr.ru%2Fpost%2F163689%2F))解析 USB 设备端。这似乎是项目的最大部分，但他仍然需要路由器上的驱动程序来与设备接口。这让他进入了[USB 级驱动程序的世界](http://habrahabr.ru/post/163861/) ( [翻译为](http://translate.google.com/translate?sl=auto&tl=en&js=n&prev=_t&hl=en&ie=UTF-8&eotf=1&u=http%3A%2F%2Fhabrahabr.ru%2Fpost%2F163861%2F))。它甚至包括在 OpenWRT 的内核中构建图形支持。拼图的最后一块是[编写一个帧缓冲区](http://habrahabr.ru/post/164635/) ( [翻译为](http://translate.google.com/translate?hl=en&sl=auto&tl=en&u=http%3A%2F%2Fhabrahabr.ru%2Fpost%2F164635%2F))来帮助调节屏幕的输出。结果非常好，他甚至可以用 ScummVM 玩游戏。休息后在片段中自己看吧。

[https://www.youtube.com/embed/9A8V1dniLlQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/9A8V1dniLlQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)