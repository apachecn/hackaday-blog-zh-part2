# 3D 打印机挤出机的精确温度控制

> 原文：<https://hackaday.com/2013/09/19/accurate-temperature-control-of-your-3d-printer-extruder/>

[![](img/ac4d03b251f454b6c2d9ce09ba78efd6.png)](http://hackaday.com/wp-content/uploads/2013/09/img_20130904_184235_edit.jpg)

[Tim]正在建造一台 3D 打印机，并以此为借口尽可能多地学习。他解决的第一个大问题是精确的温度控制，因此他写了一篇关于如何表征 QU-BD 挤出机热端的热特性并使用该信息创建加热器控制算法的[有趣的文章](http://www.wildcircuits.com/2013/09/accurate-temperature-control.html)。

文章从一个基本的热模型及其相应的公式开始。[Tim]然后进行了几次测试，在测试中，他在打开和关闭加热器的同时测量加热器和挤出机尖端的温度。这使他能够计算出设计控制算法所需的几个模型参数。最后，他调整了他的公式，以预测短期未来，这样他就可以知道什么时候应该激活加热元件。结果，他的体温现在被精确地控制在 200 摄氏度+/-1 摄氏度的范围内，这正是他的目标。