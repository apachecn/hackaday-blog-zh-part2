# 创造多媒体电梯之旅

> 原文：<https://hackaday.com/2012/05/04/creating-a-multimedia-elevator-ride/>

![](img/db91a60d43f845e2195f2d678fb22267.png "video-on-an-elevator")

[Ben Peoples]在剧院电子公司工作。听起来很有趣，这是他做的事情的一个例子。我们不确定这个装置用于什么活动，但是如果乘坐电梯需要一些华而不实的东西，只要想想派对房间看起来会是什么样子。电梯天花板上的高清电视屏幕[在电梯上升或下降](http://www.trinculosattic.com/2012/05/show-business-has-its-ups-and-downs/)时播放不同的片段。[Ben]面临的挑战是找到一种方法让它工作，而不需要接入电梯电子设备，也不需要任何按钮。

第一次尝试用加速度计来检测电梯的行程。这种方法的问题在于，加速度计只检测加速度的变化，这种方法很容易出错。[本]切换到一个反射传感器，表现相当好。由于大多数传感器只能在大约八分之一英寸的范围内工作，他最终用一个 LDR 和几个琥珀色的发光二极管构建了自己的传感器。

[via [Reddit](http://www.reddit.com/r/arduino/comments/t6olv/show_business_has_its_ups_and_downs_an/)