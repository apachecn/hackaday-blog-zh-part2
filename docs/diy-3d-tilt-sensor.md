# DIY 3D 倾斜传感器

> 原文：<https://hackaday.com/2014/07/01/diy-3d-tilt-sensor/>

如果你试图检测一个物体的方向，有时你真的不需要 6 自由度陀螺仪和加速度计。见鬼，如果你只需要检测一个物体是否倾斜，你可以花几分钱买到一个简单的“管中球”倾斜传感器。[tamberg]喜欢这个想法，但他需要一个能在 X、Y 和 Z 轴上工作的倾斜传感器。在简单倾斜传感器的“管中球”结构的基础上，[他设计了一个激光切割 3D 倾斜传感器](http://hackaday.io/project/906)，它可以完成 30 美元 IMU 的所有工作。

这种倾斜传感器的基本设计非常简单——只是一个八面体，每个顶点有四个钉子作为开关触点。一个铝球在这个奇妙的装置里敲来敲去，根据它的方向关闭钉头开关。简单，三维版本的球管倾斜传感器。

为了将倾斜数据传递给外界，[tamberg]正在使用一个 Adafruit 蓝牙模块，每个角落的两个钉子都连接到一个引脚上。只需一点点代码，这个 3D 倾斜传感器就变成了一个控制 RGB LED 的六路开关。下面的视频。

[https://embedr.flickr.com/photos/14034330334](https://embedr.flickr.com/photos/14034330334)