# 如何称一根睫毛

> 原文：<https://hackaday.com/2015/02/12/how-to-weigh-an-eyelash/>

所以你是一名拳击手，你的体重只比你通常的体重等级多了 80 微克。你需要拔掉多少根睫毛才能重返拳台？或者也许你正在追随最新的饮食时尚，“微烹饪”，一份食谱需要 750 微克的糖，你需要知道那是多少谷物。你需要一个微克级的。

好吧，我们实在想不出一个好的理由来称一根睫毛，除了说你称过。无论如何，不是一个 T1 而是 T2 的两个 T3 的 YouTube 视频向你展示了如何在一个面板式仪表的机械装置中建立一个微克天平。你知道，就是那种在数字时代之前用的摆动指针的那种？

面板式电表本质上是永久磁铁(一个[电流计](https://en.wikipedia.org/wiki/Galvanometer))中弹簧上的电磁铁。当没有电流流过电磁铁时，弹簧将指针拉向最左侧。当你推动电流通过电磁铁时，它会被固定的永久磁铁吸引，对抗弹簧，并将指针拉向右边。电流越大，拉力越大。

第一个链接来自德州仪器的 Paul Grohe，演示了基本原理。安排好仪表，使臂落入光遮断器的路径中，然后建立一个小电路，使更多的电流通过仪表的电磁铁，当臂中断光束时，将臂拉回来。

当手臂落下时，因为你把一根睫毛放在上面，它会打断光束，光束驱动更多的电流把手臂拉回来。这将来回摆动，直到它的手臂刚好打断横梁。然后你可以读出支撑它所需的电流，这个电流和重量成正比。

[https://www.youtube.com/embed/n90whRO-ypE?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/n90whRO-ypE?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

来自[应用科学]的第二个链接更加详细。[Ben Krasnow]重建了[Grohe]的电路，研究了天平的线性度(良好)和稳定性(一般),并演示了如何用纸方块校准天平。他还发现，由于静电荷，他的塑料外壳正在拉动机械装置。

[本]很容易就能从他桌子上的几块钱的零件中得到大约 10 微克的精度。此外，他亲自动手描述和调试设置的方式真的让我们很感动。

[https://www.youtube.com/embed/ta7nlkI5K5g?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/ta7nlkI5K5g?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

(而且答案都是:80 微克是两根睫毛；十粒糖重约 750 微克。)

感谢[Travis Swaim]发送链接给我们。