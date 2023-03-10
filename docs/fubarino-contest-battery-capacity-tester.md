# Fubarino 竞赛:电池容量测试仪

> 原文：<https://hackaday.com/2013/12/16/fubarino-contest-battery-capacity-tester/>

![fubarino-contest-battery-capacity-tester](img/bc7945b00e060a1236840ce736397b1b.png)

这里有一个项目，几年前我们很遗憾地错过了。幸运的是[布莱恩]掸掉了它的灰尘，并在固件中添加了一个复活节彩蛋，以便将其包括在 Fubarino 竞赛中。该设备是一个可充电电池容量测试仪。它通过大约 1 瓦的负载电阻对镍氢电池或镍镉电池进行放电。[Brian]在他的文章中讨论了硬件无法支持 14500 个锂离子电池。他包含了足够的信息，如果您想启用此选项，您可以知道如何对电路进行更改。

有一个 MOSFET 用于切换三个电池位置中的每一个。ATmega168 每秒钟从电池中读取一次读数。它在诺基亚 5510 手机屏幕上显示状态信息。这是他选择注入黑客日 URL 的地方。当一个细胞的放电完成时，上面的图像会滚动到屏幕上，并停留一小段时间。休息之后自己看吧。

[https://www.youtube.com/embed/7HhEzlcrpjY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/7HhEzlcrpjY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

* * *

这是 Fubarino 比赛的参赛作品。在 2013 年 12 月 19 日之前提交您的参赛作品，您将有机会获得微芯片推出的 20 个 [Fubarino SD 板](http://www.microchip.com/stellent/idcplg?IdcService=SS_GET_PAGE&nodeId=1406&dDocName=en566210)中的一个作为奖品！