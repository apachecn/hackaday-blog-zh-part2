# 自动转盘摄影

> 原文：<https://hackaday.com/2012/04/11/automated-turntable-photography/>

[Muris]有一个朋友在网上卖东西。这位朋友想要一种简单的方法来制作产品的旋转图像，并请他帮忙。他的劳动成果是[这个驱动转台和控制摄像机的基本单元](http://www.elektronika.ba/832/turntable-photography-equipment/)。

转盘的第一次迭代由软驱中的步进电机驱动。一个光盘被直接安装在电机主轴上，但结果有点差。这是因为电机的分辨率相当低，每转 200 步。这不允许平滑的动画，而且系统中有很多振动。你在上面看到的齿轮传动系统的升级包括用一个旧扫描仪的马达替换掉那个马达。现在它每转 1200 步，振动消失了。

在底座上看到的连接器是 USB、输入电源和快门控制。[Muris]写了一个程序来控制基地内部的 PIC 16F628A。该程序通过 USB 发送命令，并具有每次旋转的帧数、旋转方向等参数。根据需要进行设置，将产品放在转盘上，然后点击开始。不幸的是，没有这方面的视频，因为[穆里斯]一完成就把它给了他的朋友。我们猜测他没有拿回来的事实意味着它工作得很好。

如果你不介意一些粗糙的边缘和暴露的线路，你可以很快地[组装出自己的系统](http://hackaday.com/2011/06/22/photo-hardware-had-automatically-produces-rotating-gifs/)。