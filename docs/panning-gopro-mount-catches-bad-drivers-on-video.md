# 平移 GoPro 挂载捕捉视频上的坏驱动程序

> 原文：<https://hackaday.com/2014/03/14/panning-gopro-mount-catches-bad-drivers-on-video/>

![gopro-mount](img/1c64d938752a1cb10c7c3eb96e45752d.png)

[克里斯]一定住在一个有很多糟糕司机的社区。他建造了这个[电动平移 GoPro 支架](http://hackaday.io/project/413)，这样他就可以记录并与世界分享他邻居的移动不幸。他从一个定制的铝制框架开始。框架夹在吸盘安装扶手杆上。股票 GoPro 安装在一个加工的 HDPE 圆盘上，由 NEMA 11 步进电机旋转。[克里斯]使用了一个 [Pololu A4988](http://www.pololu.com/product/1182) 步进电机驱动器来处理线圈。最初，他使用 Arduino 为步进驱动器产生脉冲。虽然他是一个真正的黑客粉丝，但他认为 Arduino 太过了，于是拿出了一个 [555 定时器](http://en.wikipedia.org/wiki/555_timer_IC)。DPDT 开关启动 555 并控制步进驱动器的方向输入。所有的电子设备都整齐地装在一个小的项目箱里，这个项目箱可以兼作手控器。

在准备试驾时,[Chris]发现他只能锁定汽车弧形天窗上的一个吸盘。考虑到 GoPro 的重量很轻，一个吸盘大概就够了。为了安全起见，[克里斯]在天窗下面加了一条绳子。

我们认为步进电机是这个项目的好选择。由于电机是直接驱动，没有齿轮剥离。步进器的保持扭矩也可以在高速公路上保持相机指向正确的方向。由于没有电线直接将 GoPro 连接到汽车上，【克里斯】可以将相机旋转 360 度而不用担心缠结。验证摄像头的方向只是通过汽车的天窗向上看的事情。点击休息时间，查看[Chris 的]相机安装的效果。

[https://www.youtube.com/embed/3kZ-kx1SKD0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/3kZ-kx1SKD0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)