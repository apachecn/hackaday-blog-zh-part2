# 多旋翼飞机的超级简单万向架在复杂性面前笑了

> 原文：<https://hackaday.com/2014/05/29/super-simple-gimbal-for-multi-rotor-aircraft-laughs-in-the-face-of-complexity/>

![Super Simple Multi Rotor Gimbal](img/c1320f5ebee648bd81615498d3eb13a9.png)

在你新造的多用途直升机首次飞行后，你会立即想要增加一个照相机。这一系列事件遵循物理定律，就像重力一样可以预测。仅仅通过一个固定支架把相机绑在上面可能在技术上解决了这个问题，但它产生了另一个问题。改变飞行方向会导致多直升机倾斜和翻滚。如果多直升机倾斜和翻滚，你的相机也会倾斜和翻滚。这就是万向架派上用场的地方，它将摄像机调整到与飞机方向相同和相反的方向。如果飞机向前倾斜，万向节将摄像机向后倾斜相同的角度。结果是一个稳定的相机捕捉一些甜蜜的视频。

rcgroups.com 的 SSG 团队已经发明了他们所谓的超级简单万向架。他们的设想是一种价格低廉、易于制造并且给飞机增加最小重量的万向架。在一个正常的万向架上，有两个马达或伺服系统，每个都专门控制一个运动轴。在 SSG 上，有两个伺服系统，但它们不会彼此独立运行。摄像机安装在一个平板上，平板的一端由一根硅胶管支撑，硅胶管成为系统的支点。该板的另一侧由两个连杆(也由硅胶管制成)支撑，连杆本身连接到伺服系统。如果两个伺服系统都向上移动，摄像机就会向下倾斜。如果右伺服向上移动，左伺服向下移动，则摄像机向左倾斜。

那么，伺服系统是如何知道该做什么以及何时做的呢？一些多旋翼飞行控制板有直接连接伺服系统的输出。控制板使用机载陀螺仪和加速度计来感应飞机的运动，并确定相机的移动量。

如果你有兴趣为自己制作一个，请点击上面的链接找到你需要的一切。感谢 SSG 团队如此出色地记录了这个项目。如果一个别致的无刷电机万向架更符合你的风格，看看这个你可以用 3D 打印机打印出来的。

[https://www.youtube.com/embed/KPBL4pPEzNI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&start=313&wmode=transparent](https://www.youtube.com/embed/KPBL4pPEzNI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&start=313&wmode=transparent)