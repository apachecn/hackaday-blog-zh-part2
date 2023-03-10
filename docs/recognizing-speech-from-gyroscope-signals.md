# 电话陀螺仪信号可以窃听你的谈话

> 原文：<https://hackaday.com/2014/08/24/recognizing-speech-from-gyroscope-signals/>

[![](img/ad643f6d70af5554db7720c4a86ef0d2.png)](https://hackaday.com/wp-content/uploads/2014/08/mems.png)

陀螺仪是一种用于测量方向的设备，通常可以在现代智能手机或平板电脑中找到，以实现丰富的用户体验。来自斯坦福的一个团队成功地从只分析陀螺仪信号的[中识别出简单的单词](http://crypto.stanford.edu/gyrophone/files/gyromic.pdf) (PDF 警告)。基于 MEMS 的陀螺仪(使用科里奥利效应)的[复杂的内部工作方式](http://en.wikipedia.org/wiki/MEMS_gyroscope#MEMS_gyroscope)和 Android 软件限制只允许团队只能嗅探 200Hz 以下的频率。因此，这可以解释使用自定义识别算法所达到的平均 12%的单词识别率。然而，这可能仍然足以让你重新考虑安装一个不一定需要访问机载传感器才能工作的应用程序。有趣的是，该论文还指出，意法半导体目前在智能手机/平板电脑陀螺仪领域拥有 80%的市场份额。

在同一个话题上，你可能有兴趣看看几年前我们报道过的基于陀螺仪的智能手机键盘记录攻击。