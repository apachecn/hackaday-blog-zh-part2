# 清洁微型自平衡机器人

> 原文：<https://hackaday.com/2013/05/13/clean-and-minimal-self-balancing-robot/>

verti bot[是一个自平衡机器人项目](http://madebyfrutos.wordpress.com/2013/05/02/vertibot/)，目的是探索传感器如何与一些 PID 算法结合工作。

[米格尔]没有把任何额外的东西放进建筑里。但你不得不承认这让它看起来很有趣。几乎没什么，但是，正如你在休息后的剪辑中看到的，他完成了他设定的一切。

[的车身和车轮是 3D 打印的](http://www.thingiverse.com/thing:83091)，轮胎上的黑色条纹有助于增加牵引力。请注意身体中心的连接，这使他能够通过两个阶段打印来制作更长的部分。在电子方面，他使用的是 Arduino Nano。一个电平转换器让它与用于检测运动的 6 自由度 IMU 板通信。三个电位计为他提供了调整 PID 环路的方法，而无需重新刷新任何代码。当然，由于混合了蓝牙模块，还可以选择远程控制它。

[https://www.youtube.com/embed/A5KtT4GVpx8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/A5KtT4GVpx8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)