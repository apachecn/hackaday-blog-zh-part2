# DIY 风火轮赛车计时器

> 原文：<https://hackaday.com/2015/01/19/diy-hot-wheels-drag-race-timer/>

[Apachexmd]想为他三岁儿子的生日聚会做点好玩的事。知道赛车有多酷，他选择制造自己的[风火轮赛车计时器](http://imgur.com/a/K1Lbf "Hot Wheels drag race timer")。他也没有走捷径。在这个项目中，他测试了自己的电子技术和 3D 打印技术。

该系统有两个主要组件。首先，是起跑门。为了公平的比赛，所有的车都必须同时离开大门，所以[Apachexmd]需要一种电子控制的方法。他的解决方案是使用一个连接到铰链的伺服系统。铰链有四个机器螺丝，每辆车一个。当伺服器朝一个方向旋转时，铰链会将螺丝从轨道上的孔中推出。这可以防止汽车在下坡行驶。当启动按钮被按下时，螺丝被拉回，汽车可以自由地让重力接管。

第二个组成部分是终点线。轨道下面是四个激光二极管。这些光线通过轨道上的钻孔向上照射。四个光电晶体管安装在上面。这些充当传感器，检测激光束何时被汽车阻断。它的工作原理类似于[激光绊线报警系统](http://hackaday.com/2011/04/19/laser-trip-wire-the-bare-essentials/ "Laser trip wire")。传感器朝下，用黑色胶带覆盖，以阻挡额外的光噪声。

轨道上方还有八个 7 段显示器；每辆车两个。该系统能够记录汽车通过终点线的顺序。当比赛结束时，它会显示每辆赛车在相应赛道上的名次。该系统还以秒为单位记录获胜赛车的时间，并在显示屏上显示出来。

该系统运行在 Arduino 上，几乎完全由定制设计的 3D 打印组件构建而成。由于所有的组件都设计得非常完美，最终的结果是一个非常光滑的比赛计时器。也许下一个[Apachexmd]可以添加一个[雷达枪](http://hackaday.com/2014/08/18/hot-wheels-toy-turned-radar-detector/ "Hot Wheels radar gun")来记录最高速度。看看下面的视频，看看它的作用。

[https://www.youtube.com/embed/_Uf9mUJJ-9M?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/_Uf9mUJJ-9M?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)