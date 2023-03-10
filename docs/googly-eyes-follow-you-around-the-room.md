# 眼睛在房间里跟着你

> 原文：<https://hackaday.com/2015/06/04/googly-eyes-follow-you-around-the-room/>

如果你正在寻找下一个令人毛骨悚然的万圣节装饰，或者只是想第一次尝试 OpenCV，这个下一个项目将会涵盖你。[格伦]用一些伺服系统和一些非常强大的软件做了一双巨大的眼睛，在房间里跟着你。

该项目分为三个部分。在第一部分中，[Glen] [自己建模并制造眼睛](http://bikerglen.com/blog/build-a-pair-of-robotic-googly-eyes/)，包括安装最终将移动它们的伺服电机。第二部分涉及[一个 Arduino 和控制伺服系统的电源](http://bikerglen.com/blog/bringing-the-robotic-googly-eyes-to-life/)，第三部分使用 [OpenCV 跟踪人脸](http://bikerglen.com/blog/tracking-people-with-the-googly-eyes-and-opencv/)。

如果您是 OpenCV 的新手，那么项目的这一部分可以说是最有趣的；[格伦]用这个软件包来识别不同的面孔。从那里，计算机挑选出最突出的脸，并向 Arduino 发送命令，将眼睛移动到适当的位置。该项目非常详细，从 Arduino 代码到安装 Ubuntu 到第一次运行 OpenCV！

我们之前介绍过[Glen]的一些项目，比如他的[FPGA 驱动的 LED 墙](http://hackaday.com/2014/04/11/beaglebone-black-and-fpga-driven-led-wall/)，很高兴看到他仍然在做伟大的事情！

[https://www.youtube.com/embed/ez7bBb92yZM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/ez7bBb92yZM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)