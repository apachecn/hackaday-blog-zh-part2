# 使用 MSP430 的轻量级 Web 服务器

> 原文：<https://hackaday.com/2012/07/17/lightweight-web-server-using-the-msp430/>

![](img/4e831a3ccad8e9cfa08428d70c3f408f.png "430")

需要一个微型网络服务器吗？[Rob]在 43oh 论坛上[为非常流行的 TI MSP430 微控制器制作了一个以太网增强包](http://www.43oh.com/forum/viewtopic.php?f=35&t=2529)。如果这还不够的话，[Rob]还将 MSP430 和以太网控制器放在一起，组成了一个由电池供电的一体化解决方案。除了仅容纳 5k 闪存的 web 服务器，我们还要说[Rob]为遥感和数据记录提供了一个非常好的解决方案。

对于支持以太网的 430，[Rob]选择使用 [WIZnet W5200 以太网控制器](http://www.wiznet.co.kr/sub_modules/en/product/Product_Detail.asp?cate1=5&cate2=38&cate3=0&pid=1144)。该芯片通过 SPI 接口与 430 通信，并具有支持 TCP、UDP 和 PPPoE 的硬件 TCP/IP 堆栈，将 430 的所有底层内容卸载到以太网控制器上。

休息过后，有两段视频显示了[Rob]展示他的微型网络服务器。一些简洁的功能包括 430 的完整内存转储，以及通过 HTML 页面读取所有引脚的状态。如果你正在寻找一种通过以太网收集数据的方法，我们不认为你能比[Rob]的基于 430 的微型网络服务器做得更好。另外，如果你想通过互联网控制一些设备，[Rob]提供了一些用于照明或电器的光隔离器。

代码可以在 43oh 论坛页面上找到，但是[Rob]说他会把它清理干净并放到一个 Git 中。

[https://www.youtube.com/embed/2Xu4rIqPUP0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/2Xu4rIqPUP0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)
[https://www.youtube.com/embed/W_Ng5Kc_LqY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/W_Ng5Kc_LqY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)