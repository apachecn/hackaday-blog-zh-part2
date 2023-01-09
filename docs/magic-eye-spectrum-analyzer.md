# 魔眼光谱分析仪

> 原文：<https://hackaday.com/2013/01/14/magic-eye-spectrum-analyzer/>

![its goddamned magic](img/fc978a5f11711da8254d9ce300a51ecb.png)

如果 Nixies 还不够酷，也许是时候升级到魔眼管了。

像尼克斯和德卡龙一样，电眼管是显示管。与数码管中的字母数字字符或旋转光点不同，魔眼管是条形图或“吃豆人”显示器，用于在非常昂贵的收音机上显示电台的信号强度。

在用电子管做了几次实验后，[sylvain]觉得用魔眼电子管做点什么会很酷。他采购了八个垂直的“条形图”电眼管，并建造了一个音频频谱分析仪。

更困难的事情之一是计算每个频带的功率水平。有几个图形均衡器 ic 可用，但[sylvian]决定走老派，更难的方式，把一个 FFT 算法在 ATMega624 上。

一件令人印象深刻的作品，在一个漂亮的电子管立体声系统旁边看起来会很惊人。