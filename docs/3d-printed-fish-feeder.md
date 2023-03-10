# 3D 打印喂鱼器

> 原文：<https://hackaday.com/2015/02/27/3d-printed-fish-feeder/>

[Helios Labs]最近发布了他们的第二版 [3D 打印喂鱼器](http://helioslabs.blogspot.com/2015/01/arduino-3d-printed-fish-feeder-v2.html "3D printed fish feeder")。这个系统被设计成一天喂两次鱼。该设计由九个独立的 [STL 文件](https://www.thingiverse.com/thing:653522/#files "Thingiverse")组成，可以安装到挂在水产养殖系统鱼缸上方的花盆上。不过，修改设计使之适用于普通鱼缸可能不需要太多。

这个系统非常简单。这个装置主要是一个装鱼食的盒子或漏斗。底部是一个 3D 打印的螺旋钻。螺旋钻被超级胶水粘到一个伺服机构的齿轮上。9g 伺服很小，并且带有内部限制器，只允许它旋转大约 180 度。伺服系统必须打开，限制器必须移除，以使[能够进行 360 度旋转](http://hackaday.com/2008/07/14/modifying-a-servo-for-continuous-rotation/ "Hacking servos for continuous rotation")。伺服系统由 Arduino 控制，可以直接安装在 3D 打印的外壳上。螺旋钻的设计可以防止鱼食意外进入电子设备舱。

你可能会认为这个项目将使用实时时钟芯片，或者可能与计算机接口来保持时间。相反，代码只是在插入时喂鱼一次。然后，它使用“延迟”功能，以便在第二次喂鱼之前等待一段设定的时间。在示例代码中，这被设置为 28，800，000 毫秒，即 8 小时。在第二次喂鱼之后，再次调用延迟函数，以便等到最初的开始时间。