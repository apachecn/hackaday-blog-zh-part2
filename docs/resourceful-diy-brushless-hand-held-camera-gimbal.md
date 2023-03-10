# 足智多谋的 DIY 无刷手持相机万向节

> 原文：<https://hackaday.com/2015/03/28/resourceful-diy-brushless-hand-held-camera-gimbal/>

在拍摄视频时拿着摄像机可能会导致完成的镜头有一些严重的抖动。幸运的是，我们有一些解决这个问题的方法，如被动稳定凸轮稳定器或主动电机驱动万向节。[Oscar]想要一个运行平稳的无刷电机万向架，但又不想花大价钱购买，所以他出去[建造了自己的](http://blog.oscarliang.net/build-brushless-camera-gimbal-handheld-quadcopter/)。

[奥斯卡]没有数控机床或 3D 打印机来帮助他的建设。他用胶合板和五金店的支架，用简单的手工工具制作了万向架。在他的 build 帖子中，他谈到了保持万向节的旋转轴与相机镜头保持一致是多么重要，以及他为实现这一目标做了什么。轴和镜头的对齐确保了视频的稳定性，同时万向节进行调整以保持摄像机的角度恒定。

[Oscar]购买了无刷电机和电机控制器，其中包括一个位于独立 PCB 板上的陀螺仪传感器。陀螺仪安装在相机支架上，并将倾斜信息发送回控制器，然后控制器移动无刷电机以保持相机水平。最终的项目进行得相当不错，尽管[Oscar]承认他仍然想把控制器中的 PID 设置调得更好一点。休息后，请查看视频，其中将稳定的摄像机与未稳定的摄像机进行了比较。

[https://www.youtube.com/embed/oro9B0hXGto?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/oro9B0hXGto?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)