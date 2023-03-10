# 裸机 Arduino 红外接收器

> 原文：<https://hackaday.com/2014/05/30/bare-bones-arduino-ir-receiver/>

![TV Remote](img/cc66b3de1b208cc303b1af7099073715.png)

老式红外遥控器是与您的项目交互的好方法。[AnalysIR]最新的一篇博客文章讲述了创建一个基于 Arduino 的红外接收器的最简单的方法，这比以往任何时候都更容易将那个旧遥控器很好地用于[。](http://hackaday.com/2014/05/26/ancient-tv-remote-becomes-a-cnc-pendant/)

由于他们的第一篇红外接收器帖子[银弹红外接收器](http://www.analysir.com/blog/2014/05/04/silver-bullet-oscilloscope-infrared-receiver/) , [AnalysIR]决定写一篇关于在 Arduino 上使用红外的快速帖子。零件清单包括一个 Arduino、两个电阻和一个 IR 发射器。没错，一个发射器。当 LED (IR 或其他)反向偏置时，它可以充当光传感器。使用这种方法的主要区别在于，当使用更普通的调制 IR 接收器模块时，IR 信号不会像通常那样反转。还提供了启动和运行所需的所有 Arduino 代码。使用这种配置的主要限制是，遥控器需要非常靠近红外发射器才能接收信号。

你会用你的旧[电视遥控器](http://hackaday.com/2011/09/06/playing-snake-with-a-tv-remote/)控制什么？将这种电路连接起来会很有趣，这样一个红外发射器就可以同时作为发射器和接收器。去试一试吧，然后[让我们知道](http://hackaday.com/contact-hack-a-day/)进展如何！