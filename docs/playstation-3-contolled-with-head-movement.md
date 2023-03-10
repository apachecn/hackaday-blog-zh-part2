# 用头部运动控制的 PlayStation 3

> 原文：<https://hackaday.com/2013/07/05/playstation-3-contolled-with-head-movement/>

我们对黑客如何运用他们的技能开发新的适应性技术越来越感兴趣。这是定制控制技术帮助[Steven]重返游戏的另一个很好的例子。肌肉萎缩症的影响使他无法使用 PS3 控制器。但是在与[约翰·希梅尔]搭档后，他又能玩游戏了，这多亏了头部运动控制系统。

[John]观察了[Steven]与手边的辅助技术互动的方式。他可以用一根手指驾驶轮椅，通过移动头部与电脑互动。电脑检测到他帽沿上的一个标记。[John]使用 Java 从计算机获取输入，并将其发送到通过 USB 连接的 Arduino 板。Arduino 有一个 USB Bit Whacker 板，让它也可以连接到 PS3 作为控制器。在上图中，你可以看到电脑屏幕上的每个控制器按钮都有一个 GUI。[John]移动他的头来选择一个控制，并用他的手指点击一个按钮来启动它。

如果你喜欢这个，看看我们最近看到的其他辅助游戏技巧。

[通过[控制器项目](http://thecontrollerproject.com/head-tracking-ps3-controller/)