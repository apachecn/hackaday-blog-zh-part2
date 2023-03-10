# 用心率测量冥想

> 原文：<https://hackaday.com/2013/03/20/measuring-meditation-with-a-heart-rate/>

![meditation](img/703c1d28419de097000539b7984e6b0c.png)

这些年来，我们已经看到了相当多的构建试图窥视用户的大脑，并预测他们的精神状态。无论目标是诱导清醒梦还是仅仅减少焦虑，我们总是对你可以用生理测量来检测情绪的许多方法印象深刻。[Kirk]几个月来一直在测量自己的生理状况，发现冥想期间最大的变化是心率的变化。利用这种算法，他[制作了一个球体，当他冥想的时候](http://www.kpkaiser.com/entrepreneurship/building-a-meditation-controlled-orb/)它会改变颜色。

构建的硬件使用蓝牙 LE 心率监测器连接到智能手机，与电动 Imp 通信。处理完心率数据后，Imp 会触发一个由 Arduino 控制的 RGB LED 灯条。结果是一个塑料球体，每当用户表现出某种正念时就会发光，与无意识浏览互联网产生的算法相互参照。