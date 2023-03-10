# 当它听到大的噪音时，颤动的衣服震动

> 原文：<https://hackaday.com/2012/08/13/flutter-dress-vibrates-when-it-hears-loud-noises/>

[![](img/bcb673fe7837a8effe7505a8dc1d9807.png "flutter")](http://hackaday.com/wp-content/uploads/2012/08/flutter.png)

许多有听力障碍的人家里有辅助设备，每当消防车经过、警铃响起或门铃响起时，辅助设备就会闪烁灯光。除了一只助听狗，这些设备在户外都没用，这就是[哈雷]的[飘动礼服发挥作用的地方](http://halleyprofita.wordpress.com/projects/)。Flutter 将麦克风和微控制器缝在衣服上，以听取周围的环境，并使用小型振动马达，每当检测到大声的声音时，就挥舞小布传单。

在为 Flutter (PDF)撰写的[文章中，【Halley】告诉我们她使用了四个微控制器来检测周围的声学环境。每个微控制器将来自麦克风的信号传递到缓冲器中，在缓冲器中对声音数据执行 FFT。由此可以确定噪音的响度和频率，以及飞行时间计算的方向。一旦完成，每个微控制器就会根据声音的大小和方向来驱动裙子上的一个小型振动马达。](http://correll.cs.colorado.edu/wp-content/uploads/ISWC2012_AdjunctProceedings.pdf)

与所有针对听力受损者的辅助技术一样，聋人文化的观点总是认为这些发明是在给某人强加残疾。[Halley]的飘动礼服征求了一些有听力障碍的家庭成员的意见，并从社区成员那里获得了一些积极的反馈。干得好，我们可以看到为什么它在 2012 年可穿戴计算机设计展国际研讨会上赢得了最佳展示奖。