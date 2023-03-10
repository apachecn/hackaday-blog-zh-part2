# 易于构建的可编程脚踏开关

> 原文：<https://hackaday.com/2013/02/26/simple-to-build-programmable-foot-switches/>

![programmable-footswitches](img/b896c4dc95206cb3f5be4b4bffc68b5d.png)

你的手在键盘和鼠标之间做了很多工作，你为什么让你的脚这么懒？[档案范迪]正在结束足病树懒。[他制作了这套三个脚踏板](http://www.dossierd.nl/ap_voetschakelaar_eng.html)，经历了两个版本的功能。

按钮本身是由胶合板基板制成的，每个“键”的顶部有一小块。这两个部分用一些泡沫地毯垫分开，中间有一个触觉按钮来记录点击。对此我们唯一要改变的是在开关旁边增加几个木制垫片，这样不小心砂到按钮上就不会损坏电子元件。

最初，每个按钮都焊接在一个游戏控制器上。使用按钮映射效果很好，但是最近[档案]改用 Arduino Leonardo。这是一个完美的选择。与使用旧版本 Arduino 制作的[输入设备不同的是](http://hackaday.com/2011/06/27/teamspeak-button-uses-tattoo-machine-foot-switch/), Leonardo 板可以本地注册为键盘，这使得通过编程将任何按键映射到开关变得轻而易举。

如果你喜欢这个项目，你应该看看[档案] [脚鼠标](http://hackaday.com/2012/03/07/foot-controlled-mouse-keeps-your-hands-on-the-keyboard/)以及。