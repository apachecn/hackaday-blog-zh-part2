# 无印刷电路板的谢妮钟

> 原文：<https://hackaday.com/2012/10/11/nixie-clock-without-a-pcb/>

[![](img/bc52e13799e27c1197e2c0c796daa56d.png "Lethal Nixie Cube")](http://hackaday.com/?attachment_id=87736)

寻找一种艺术的方式来构建电路？不想设计 PCB？致命数码管时钟是一种自由形式的电路，一次给你一个数字的时间。它使用 1 英寸数码管来显示数字。这由十个 MPSA42 高压晶体管驱动。IRF520 N-FET、电感和二极管用作开关电源，产生驱动数码管所需的高压。可能不致命，但是立方体里有暴露的高压。你肯定会后悔碰它。

ATMega8 用于控制时钟。它驱动数码管的各个数字，并产生 PWM 输出来切换高压电源。不幸的是，示意图已经丢失。如果你对开关电源感兴趣，它可能类似于这里解释的。

休息之后，请观看时钟的视频。

经由[危险原型](http://dangerousprototypes.com/2012/10/10/freeform-nixie-clock/ "Dangerous Prototypes")

[https://www.youtube.com/embed/06-RMMxYA1Q?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/06-RMMxYA1Q?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)