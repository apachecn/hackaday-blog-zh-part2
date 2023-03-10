# 笔迹烂？造一台机器来帮你做这件事

> 原文：<https://hackaday.com/2013/03/08/handwriting-suck-build-a-machine-to-do-it-for-you/>

![calligraphy-machine](img/4d9f7ec3f57533a7917198c9b41b5442.png)

信息时代的孩子注定会有最糟糕的书法，仅仅是因为缺乏使用。但是奥林学院的一些学生利用技术找到了解决这个问题的方法。遇见 Herald，[一台能出漂亮书法的数控机床](http://calligraphybyherald.wix.com/herald)。

该机器使用一个门架沿 X 和 Y 轴移动书写头。柔性笔尖书法笔安装在链轮上，链轮将笔尖旋转到书写表面上，注意第三轴。在大二的五人组开始实际建造之前，钻机根据他们的 CAD 图纸进行了漂亮的渲染，然后进行了调整，以确保尽可能平稳的运动。

驱动硬件非常简单，但却能产生很好的效果。它使用一个 Arduino 和三个步进电机驱动器。还有限制开关来保护硬件不受失控代码的影响。该团队设计的软件界面允许用户剪切和粘贴他们的文本，并选择字体、字体大小、对齐方式等。然后，它将文本转换成 g 代码，并将其推送到 Arduino，GRBL 包会在那里处理业务。

不要错过正在运行的设备，休息后在剪辑中写出[兰斯顿·休斯]的作品。

[https://www.youtube.com/embed/kkAE-Br1Wok?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/kkAE-Br1Wok?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)