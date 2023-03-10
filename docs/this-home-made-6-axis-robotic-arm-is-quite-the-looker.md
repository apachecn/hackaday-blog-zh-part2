# 这个自制的六轴机械臂看起来很漂亮

> 原文：<https://hackaday.com/2014/10/28/this-home-made-6-axis-robotic-arm-is-quite-the-looker/>

拥有软件工程背景的[Kris Temmerman]决定用一个[六轴机械臂](http://www.neuroproductions.be/experiments/6-axis-robot-arm/)的形式来展示他的知识……最终产品是一个令人赏心悦目的机械展示。

主要由铝原料制成，[克里斯]用从中国廉价买来的数控铣床加工他的大部分零件。这些定制的零件加上一些重型步进电机，确保了手臂在自由扭曲和沿着安装的台架滑动时的准确性。虽然手臂的大部分是金属的，但他的机器人末端的手是由 3D 打印部件制成的，可以与[克里斯]计划设计的未来附件进行切换。这个经典的夹持器由它自己的 Arduino 大脑单独驱动，控制手指中的各个伺服系统。![loadcels](img/4626044e3d2e4585a9c8b7ad1d776239.png)

每个手指都包括一些承重传感器，这些传感器是从旧秤中收集来的，因此抓取器可以在不压碎物体的情况下判断它是否抓住了物体。为了协调机器人的运动，他用 C++编写了一些好看的软件，可视化了每个关节点的反向运动学。为了演示他的作品，他制作了一个基本的演示程序，可以定位和移动随机放置在表面上的彩色积木。一个安装在手上的小型摄像机确定石块相对于机器的方向，这样手腕就可以旋转到合适的位置来拾取石块。

[Kris]在一个引人入胜的速度视频中记录了他的机器人的构建，其中包括最后完成的手臂动作的镜头:

[https://www.youtube.com/embed/cod_SNq-d6c?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&start=10&wmode=transparent](https://www.youtube.com/embed/cod_SNq-d6c?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&start=10&wmode=transparent)