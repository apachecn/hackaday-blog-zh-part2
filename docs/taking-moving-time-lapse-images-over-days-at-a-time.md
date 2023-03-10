# 一次拍摄几天的动态延时图像

> 原文：<https://hackaday.com/2012/08/31/taking-moving-time-lapse-images-over-days-at-a-time/>

![](img/ebddc94d0b798dd2dd494f48c5eecbd9.png "slow-moving-time-lapse")

看着这些百合花在延时电影中开合，真是太棒了。但更好的是，在延时事件中，可以看到相机慢慢移动。这要归功于摄影师们为此制作的一个特殊的小车。

该系统基于两个弯曲和倾斜的管道，它们构成了系统的轨道。沿着轨道行驶的小车上有一个齿轮马达，转速为每分钟 2 转。这被用作绞盘，缠绕系在轨道系统高端的细绳。当绞盘缠绕绳索时，小车沿着轨道缓慢移动。

为了在多天内完成这项工作，他们用箔纸覆盖了所有的窗户，并用荧光灯照明房间。每三分钟用一个间隔计触发照相机。Arduino 通过光敏电阻监控相机的快门 LED。图像拍摄 60 秒后，Arduino 将驱动移动小车电机几秒钟

完成的视频，以及硬件展示，可以在休息后看到。

[https://www.youtube.com/embed/Ws1TdPqRXBw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/Ws1TdPqRXBw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/MaA5Ft8Ikiw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/MaA5Ft8Ikiw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)