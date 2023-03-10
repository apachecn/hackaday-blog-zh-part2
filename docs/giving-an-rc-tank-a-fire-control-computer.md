# 给一辆遥控坦克一台火控计算机

> 原文：<https://hackaday.com/2013/06/11/giving-an-rc-tank-a-fire-control-computer/>

![tank](img/76f8139c4585d61d34610d63d1c61b34.png)

[文森特]玩遥控坦克，即使他目前的模型是二战时期的装甲，他仍然喜欢现代装备，如火控计算机和主炮的激光瞄准。他的最新项目[在 Arduino、对接收器的一些修改和红外测距仪的帮助下完成了](http://www.bricobidules.com/index.php?post/2013/03/20/Charduino%2C-phase-finale-%3A-le-t%C3%A9l%C3%A9m%C3%A8tre)(法语，[谷歌翻译](http://translate.google.com/translate?sl=fr&tl=en&js=n&prev=_t&hl=en&ie=UTF-8&u=http%3A%2F%2Fwww.bricobidules.com%2Findex.php%3Fpost%2F2013%2F03%2F20%2FCharduino%252C-phase-finale-%253A-le-t%25C3%25A9l%25C3%25A9m%25C3%25A8tre))。

库存遥控坦克包括伺服移动炮塔和必要的电子发射气枪。然而，炮塔内部机械运动的精度不是很精确，所以[文森特]不得不降低伺服系统的速度，将大的运动转化为轻微的调整。之后，他在枪管上安装了红外测距仪和激光二极管，使枪能够瞄准目标并读取其距离。

在用测距仪和激光做了一些实验后，[文森特]绘制了从在一大堆距离和目标上发射几个 bb 获得的数据。图形显示出相当的线性，在将其插入图形计算器后，他能够找到一个考虑了距离和角度的方程，因此 Arduino 驱动的火控计算机将达到目标。

从各方面考虑，这支枪的精确度令人印象深刻。[文森特]能够准确地发射 bb 型导弹，并在 5 米处击中 8×12 厘米的目标。您可以查看下面操作。

[https://www.youtube.com/embed/Lrbta4zqUyA?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/Lrbta4zqUyA?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)