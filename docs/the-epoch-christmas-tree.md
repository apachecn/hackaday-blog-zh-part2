# 新纪元圣诞树

> 原文：<https://hackaday.com/2014/12/10/the-epoch-christmas-tree/>

又到了一年中的这个时候，大厅被树装饰着，树上挂满了灯，每个在零售业工作的人都因为广播里播放的圣诞歌曲而慢慢变得疯狂。[丹]有一棵树和一束可编程的发光二极管，但仅仅将欢乐注入发光二极管带是不够的。Nerd 商必须用显示 Unix 时间戳的树提高到更高的[。](http://maniacallabs.com/2014/12/09/binary-epoch-christmas-tree/)

这个版本的灵感来自于一个早期的非基于树的版本,它在一个 32 LED 阵列上显示 Unix 时间。该建筑使用 ATMega328p 开关 led。这一次，[丹]使用了专用的 LED 控制器——all pixel——刚刚结束了[一次非常成功的 Kickstarter 活动](https://www.kickstarter.com/projects/1101128588/allpixel-usb-interface-for-all-your-led-needs/)。反过来，AllPixel 由运行[biblio pixel 库](https://github.com/ManiacalLabs/BiblioPixel)的 Raspberry Pi 控制，

该树在 32 个空格中以二进制显示当前时间戳，绿色代表“1”，红色代表“0”。树的顶端是最不重要的一点，但是万一[Dan]厌倦了在这个假期的剩余时间里树的底部完全静止不动，他可以改变顺序，使树的底部成为 LSB。

下面视频。

[https://www.youtube.com/embed/dN6QREEGXBE?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/dN6QREEGXBE?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)