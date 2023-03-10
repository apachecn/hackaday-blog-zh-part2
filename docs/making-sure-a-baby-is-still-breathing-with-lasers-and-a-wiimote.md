# 用激光和 Wiimote 确保婴儿还在呼吸

> 原文：<https://hackaday.com/2012/08/21/making-sure-a-baby-is-still-breathing-with-lasers-and-a-wiimote/>

刚刚成为一名父亲，为了弥补不用带着一个足月的婴儿，他决定用另一种方式让自己变得有用。他发明了一种检测婴儿呼吸的传感器，减轻了紧张的父母的担忧，他们想知道为什么他们的孩子如此安静。

与依赖麦克风或电容传感器的类似建筑和产品不同，[Gjoci]的建筑使用 wiimote 上的摄像头来三角测量光点并检测运动。

该产品以红外发光二极管开始，但电池很大，而且婴儿总是有可能吞下电子元件。[Gjoci]最终想到了使用 1mW 的小型激光二极管来投射光点的想法。这非常有效，因为新生儿不怎么动，所以激光照射婴儿的眼睛没有危险。

构建的其余部分只是每隔几毫秒查询一次相机，看看 wiimote 相机捕捉到的反射光的位置是否发生了变化。在两周的运行中，[Gjoci]只需响应几个错误警报，硬件根本没有崩溃。

休息之后是[Gjoci]为我们发布的三个视频，展示了呼吸检测系统的测试，警报的演示，以及全面运行的构建示例。一个非常棒的构建，我们期待这篇文章在几年后的专利纠纷中被用作现有技术的证据。

[https://www.youtube.com/embed/DO-Q38jyZhY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/DO-Q38jyZhY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent) [https://www.youtube.com/embed/f7jW8dqi06c?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/f7jW8dqi06c?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent) [https://www.youtube.com/embed/w6-rEoQkr_M?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/w6-rEoQkr_M?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)