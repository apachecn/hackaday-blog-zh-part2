# 自助运输安全管理局反向散射人体扫描仪

> 原文：<https://hackaday.com/2012/11/27/diy-tsa-backscatter-body-scanner/>

[![](img/8826e247da8251587cb108cef81fd76d.png "Backscatter Scanner Image")](http://hackaday.com/?attachment_id=90729)

[Ben Krasnow]建造了他自己版本的 TSA 人体扫描仪。这个装置通过向目标发射一束 x 射线来工作。一些光束会穿过目标，一些会被目标吸收，一些会反射回来。这些反射的 x 射线被称为“[反向散射](http://en.wikipedia.org/wiki/Backscatter_X-ray "Backscatter X-ray")，它们被捕捉以创建图像。

在[Ben]的装置中，一个旋转的圆盘将 X 射线聚焦成穿过 X 轴的弧形光束。磁盘沿 Y 轴移动以填充扫描。在磁盘组件上，有一个电位计来测量光束的 y 轴位置，还有一个光学传感器来触发示波器，对准图像的左右两侧。使用这两个传感器，示波器可以重建扫描的 X-Y 图。

为了检测 x 射线，磷屏将反向散射的 x 射线转化为可见光，光电倍增器放大光源。一个简单的放大电路将光电倍增器连接到一个示波器上，控制每个点的亮度。

结果与美国运输安全管理局的版本非常相似，而且[Ben]设法从一项[专利](http://www.google.com/patents/US5181234 "patent")中学到了许多关于该系统的知识。这并不是我们看到的第一台人体扫描仪，几年前【杰里·埃尔斯沃斯】[制造了一个微波版本](http://hackaday.com/2010/12/03/make-your-own-tsa-naked-scanner/ "Microwave Naked Scanner")。

令人印象深刻的建设做了一个伟大的工作，教学的基础反向散射成像。[Ben]将在[EHSM](http://ehsm.eu/ "EHSM")谈论这个项目，如果你 12 月 28 日至 30 日在柏林，你应该去看看。休息之后，看[本]的机器扫描一只穿着圣诞毛衣的火鸡。

[https://www.youtube.com/embed/H7ldYhzKAp4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/H7ldYhzKAp4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)