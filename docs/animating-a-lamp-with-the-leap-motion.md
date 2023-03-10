# 动画带跳跃动作的灯

> 原文：<https://hackaday.com/2013/07/11/animating-a-lamp-with-the-leap-motion/>

![leap](img/8967e2ca9acd326611b90c3780186dca.png)

Leap Motion 是一个非常酷的设备，但迄今为止我们还没有看到很多与物理设备交互的应用。[Xavier]想要用手控制一个可爱的伺服动画台灯，在 Leap 和 Arduino 的帮助下他做到了。

Leap Motion API 有一个方便的特性，可以通过 websocket 输出所有数据。这是一种非常简单的方法，可以用最少的开销来传递手的位置，只需要一点 Node.js，只需要两行代码就可以将 Leap 连接到 websocket 服务器。

有了 web 服务器上的 Leap 数据，剩下唯一要做的事情就是将它下载到 Arduino。同样，[Xavier]使用了 Node.js，这次是以基于 Javascript 的 Arduino 框架 [johnny five](https://github.com/rwldrn/johnny-five) 的形式。之后，在[Xavier]的皮克斯启发的灯中，将数据从跳跃映射到伺服运动就是一件简单的事情。

下面的构建视频。

[https://player.vimeo.com/video/68530396](https://player.vimeo.com/video/68530396)