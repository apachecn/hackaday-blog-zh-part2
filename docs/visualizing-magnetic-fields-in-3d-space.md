# 在 3D 空间中可视化磁场

> 原文：<https://hackaday.com/2015/06/21/visualizing-magnetic-fields-in-3d-space/>

[约翰]正在攻读实验地震物理学的博士学位，随之而来的是成为博士的所有考验；把学生们调到这个领域中很酷的东西，并向他的顾问们展示 1970 年后创造的技术。在过去的 30 或 40 年里，他的工作中最大的进步之一就是你可以在手机中找到的所有传感器。你手机里的三轴磁力计很容易就能测量地球磁场，而这个芯片只需要几美元。为了证明这一点，[John] [建造了一个 3D 罗盘](https://hackaday.io/project/6369-3d-compass)来展示这些传感器的能力，并为大学生们做了一场漂亮的灯光秀。

[John]使用的磁力计只是一个简单的 I2C 磁力计，可以在 Adafruit 或 Sparkfun 上找到。这其实没什么特别的，但是通过一点点代码，[John]可以读取 x、y 和 z 轴上的磁场强度。

让一个微控制器吐出一堆与当地磁场相关的数字似乎并不有趣，所以[John]拿起两个 neopixel 环——一个在另一个里面，并彼此成 90 度角。这将他的磁力计和 Arduino 设置变成了一个真正的 3D 指南针。使用该设备，可以在 x、y 和 z 轴上观察到局部磁场。它看起来很酷，对本科生来说很棒，它很好地展示了你可以用小型廉价的电子传感器做什么。

[John]上传了他去年在美国地球物理联合会会议上的一次演讲的截屏。你可以看看下面。

[https://www.youtube.com/embed/OBwqT3HVbBE?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/OBwqT3HVbBE?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)