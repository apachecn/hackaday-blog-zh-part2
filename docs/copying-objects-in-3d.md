# 在 3D 中复制对象

> 原文：<https://hackaday.com/2014/01/26/copying-objects-in-3d/>

![photocopier](img/cc8c3fbd9def7cd7cd1ccc84de7e6fd4.png)

[Pulse 9]发来一个非常有趣的项目，他刚刚结束实习。这是一台 3D 影印机，它扫描一个物体，然后将该物体磨成花卉泡沫。

复印机是由随处可见的材料[Pulse]制成的——PVC、X 和 Y 轴的抽屉滑轨、结构用的丙烯酸树脂以及 Z 轴用的破损打印机零件。

为了扫描一个物体，[Pulse]将一个物体放在床上，用激光和网络摄像头扫描它。摄像机上记录的图像被输入 MATLAB。MATLAB 的输出通过串行方式发送到一个定制板，该板包含一个控制轴电机的 PIC18F4620。这个花卉泡沫路由器的主轴是一个简单的钻机；一次一层，钻头磨出不需要的泡沫，当物体完成时，这些泡沫可以被真空吸走。

下面你会看到[Pulse]的复印机演示和当地新闻对该项目的报道。如果有人愿意翻译这个故事，请在评论中畅所欲言。

[https://www.youtube.com/embed/Cst7rk9FbdU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/Cst7rk9FbdU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/8j5T-Jot_YY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/8j5T-Jot_YY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)