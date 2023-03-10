# CAMdrive 是一款开源的延时摄影控制器

> 原文：<https://hackaday.com/2015/01/29/camdrive-is-an-open-source-time-lapse-photography-controller/>

[Nightflyer]一直致力于一个他称之为 [CAMdrive](http://www.rohrhofer.org/r-tec/ "CAMdrive") 的开源项目。CAMdrive 被设计成一个用于延时摄影的多轴控制器。它目前只支持单轴，但他正在寻求帮助以扩展功能。

你可能已经熟悉了[延时摄影](http://hackaday.com/2014/12/22/a-year-long-time-lapse-camera/ "Time lapse camera")的概念。原理是你的相机在设定的时间间隔自动拍照。一个例子可以是每分钟一次。这是一个很好的方法，可以让你在很长一段时间内看到逐渐的变化。虽然这本身很有趣，但每次拍照时让相机轻微移动，往往可以让延时视频变得更有趣。CAMdrive 旨在通过提供一个框架来构建可以自动平移、倾斜和[滑动](http://hackaday.com/2010/11/30/time-lapse-camera-dolly/ "Time lapse dolly")的系统，从而在这一过程中提供帮助。

该系统被分解成独立的节点。所有节点都可以通过通信总线相互通信。电力也沿着总线分配到每个节点，使布线更容易。只要总线上的任何一个节点包含蓝牙模块，就可以通过蓝牙控制整个网络。每个节点还包括电机控制器和相应的电机。这可以是步进电机或 DC 电机。

该系统可以使用 Android 应用程序进行控制。[夜行者]目前的主要限制是应用程序。他没有太多为 Android 编写应用程序的经验，他正在寻求帮助来推进这个项目。对于那些摄影爱好者来说，这似乎是一个很有前途的项目。

[https://www.youtube.com/embed/2My9zONMP8A?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/2My9zONMP8A?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)