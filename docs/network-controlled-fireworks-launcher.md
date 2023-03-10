# 网络控制烟花发射器

> 原文：<https://hackaday.com/2013/04/13/network-controlled-fireworks-launcher/>

![rpi-fireworks-launcher](img/38932d84e888fb5601c5c85c688b32ca.png)

[托马斯]和他的朋友想通过燃放烟花来迎接新年。为了保持一个安全的距离和一点乐趣，他们建造了[这个网络控制器启动器](http://ix.residuum.org/hardware/rampe.html) ( [翻译](http://translate.google.com/translate?sl=auto&tl=en&js=n&prev=_t&hl=en&ie=UTF-8&eotf=1&u=http%3A%2F%2Fix.residuum.org%2Fhardware%2Frampe.html))。

左边的图像显示了未使用和原始状态的构建。但是在庆祝活动结束时，它看起来有点融化和烧焦了。尽管如此，对于该系统的第一次修订，它最终工作得相当好。

我们已经见过几个[远程烟火发射器，它们烧掉电阻来点燃保险丝](http://hackaday.com/2012/07/04/a-resistors-fiery-death-used-to-launch-fireworks/)。但是这个系统更具可重用性。右图显示了点燃保险丝的加热元件。年轻的读者可能不知道他们在看什么，但每辆汽车过去都至少有一个这样的电子打火机。只要给它们通上 12V 的电压，它们就会迅速变热。这就是底座上的车载电池发挥作用的地方。它通过一些机械继电器与打火机相连。

在发射器旁边的食物容器里，你会发现一个树莓 Pi，它为系统提供了网络连接。[Thomas]编写了代码，使用带有一些炸弹图标的网页作为按钮。休息之后，请观看视频，看他演示在智能手机上按下一个按钮后，这些打火机中的一个会以多快的速度发出红光。

[https://player.vimeo.com/video/63198013](https://player.vimeo.com/video/63198013)