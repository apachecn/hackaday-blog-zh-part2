# 用可视麦克风集中你的耳朵

> 原文：<https://hackaday.com/2014/08/06/focus-your-ears-with-the-visual-microphone/>

![VideoMicrophone](img/17b18e1eb98230d15395da828af1da8a.png)

一组麻省理工学院、微软和 Adobe 的研究人员已经成功地只用视频再现声音。我们发出的声音会从房间里的每一个物体上反弹回来，引起微小的振动。[可视麦克风](http://people.csail.mit.edu/mrub/VisualMic/) 利用高速摄像机和一些巧妙的信号处理从这些振动中提取音频信号。使用日常物品的视频，如零食袋、植物、聚苯乙烯泡沫杯子和水，该团队能够再现音调、音乐和语音。从光线中捕捉声音并不是什么新鲜事。[激光麦克风](http://hackaday.com/2010/09/25/laser-mic-makes-eavesdropping-remarkably-simple/)已经问世多年。不同之处在于，可视麦克风是一种完全无源的设备。不需要激光或特殊照明。

秘密在于信号处理，该团队在他们的 SIGGRAPH 论文中解释了这一点。他们使用[复杂可控金字塔](http://www.cns.nyu.edu/~eero/steerpyr/)和小波滤波器来获得局部像素运动值。这些局部值被平均为全局运动值。根据这个全局运动值，该团队能够测量低至 1/1000 像素的运动。足够的分辨率来解码音频数据。

大多数研究都是用高速摄像机进行的，这远远超出了一般黑客的预算。不过，不要绝望，该团队确实证明了消费相机也可以发挥同样的魔力，尽管结果质量较低。该团队利用了当今大多数基于 CMOS 成像器的消费相机中的[滚动快门](http://en.wikipedia.org/wiki/Rolling_shutter)。滚动快门 CMOS 传感器一次捕捉一行图像。每一行都可以以类似于高速摄像机帧的方式进行处理。当相机没有记录任何东西时，会有一些帧间间隙。即使降低了分辨率，也很容易在下面的视频中分辨出“玛丽有一只小羊羔”。

我们被这项研究震惊了，我们确信某些组织会为他们自己的使用而研究它。但是不要拿出你的[锡纸帽子](https://www.youtube.com/watch?v=w-0TEJMJOhk)。箔容器被证明是最好的声音反射器之一。

[https://www.youtube.com/embed/FKXOucXB4a8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/FKXOucXB4a8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

谢谢[扎克]！