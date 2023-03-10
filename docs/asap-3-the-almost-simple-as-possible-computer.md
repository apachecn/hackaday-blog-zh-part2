# ASAP 3–尽可能简单的电脑

> 原文：<https://hackaday.com/2013/11/04/asap-3-the-almost-simple-as-possible-computer/>

![ASAP-3 12 - LED Display](img/8fb3fcbd1fa32af5d1213aa7ad717345.png)

[Pong]加入了一个精英俱乐部，他们设计并制造了自己的计算机，其中包括一个由离散 7400 系列逻辑创建的 CPU。他的计算机是尽可能简单的计算机 3 (ASAP-3) 。ASAP-3 不是一个全新的设计。该架构基于来自[阿尔伯特·马尔维诺的书《数字计算机电子学](http://www.amazon.com/Digital-computer-electronics-Albert-Malvino/dp/0070398615)》中的 SAP 系列计算机。[Pong]看了不少“现代复古”电脑，比如 [Magic-1](http://hackaday.com/2011/07/18/building-a-computer-around-a-ttl-cpu/) 、[大乱丝 1](http://www.bigmessowires.com/bmow1/) 、[二人组](http://hackaday.com/2013/11/03/duo-basic-an-all-logic-chip-educational-computer/)。这些计算机超出了他当时的技能水平，所以他开始建立自己的系统。他的主要设计目标是能够运行一个 4 函数计算器程序。

有一件事怎么强调都不为过，那就是[Pong]通过使用大量的模拟使他的设计工作变得更加容易。他选择的工具是 Proteus 设计套件。虽然模拟不能解决所有问题，但它通常有助于验证给定的设计是否合理。ASAP-3 的指令集是基于 8085 系列指令集的微码。微码本身存储在闪存 ROMS 上。使用微码使得 ASAP-3 非常灵活。没有你需要的机器指令？没问题——写一份就行了。说到底，[Pong]有超过 100 条指令分布在 3 个闪存 ROM 芯片上。

硬件只是战斗的一半——[ Pong]发现编写软件同样具有挑战性。他用自己的机器码手写了所有的软件。这就是上面提到的模拟真正为他节省了一些时间的地方。即使进行了模拟，他仍然遇到了一些问题。ASAP-1 的时钟速度被限制在 500kHz 左右。在此之上，来自 rom 芯片的毛刺开始触发一些寄存器中的异步输入。[Pong]手头没有逻辑分析仪，所以他无法进一步追踪这个。他还发现了 [74LS181 位片 ALU](http://en.wikipedia.org/wiki/74S181) 上的进位位存在(**更新**仅模拟)问题。在某些情况下，进位不会正确传播。[Pong]通过使用 ROM 作为某些‘181 函数的查找表替代，纠正了这一问题。即使有这些限制，这仍然是一个伟大的黑客！

[https://www.youtube.com/embed/qy-nnUGPgHM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/qy-nnUGPgHM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)