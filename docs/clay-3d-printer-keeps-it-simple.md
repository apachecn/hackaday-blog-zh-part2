# 粘土 3D 打印机让它简单

> 原文：<https://hackaday.com/2014/07/28/clay-3d-printer-keeps-it-simple/>

![Clay 3D Printer](img/051e2cc04886b1e30191cc701755af7e.png)

艺术家[Jonathan]建造了一台 3D 打印机，专门用于在粘土中打印。零件数量保持在最低限度，打印机被设计成使用基本工具和初学者技能。目的是不需要使用塑料 3D 打印机来制造这种打印机。虽然这种构建的目标是粘土打印，挤出机当然可以更换为典型的塑料打印机版本。

这个 Delta 使用了相当多的 MDF。顶板和底板是 MDF，轴承座和挤出机安装板也是如此。12mm 杆单独负责顶板和底板之间的支撑，并为 LM12UU 线性轴承提供表面。这些轴承用拉链固定在 MDF 轴承架上。支撑挤出机安装板的 6 个臂由铝管和 Traxxas RC car 杆端制成。NEMA17 电机和 GT2 皮带和滑轮是用于移动机器的方法。

让粘土分散是一项棘手的任务。使用从气动分配枪中清除的部件。如果你不熟悉这种类型的工具，想想:电力填缝枪。粘土被送入可再填充的注射器，空气压缩机提供 30 psi 的压力，将粘土从喷嘴中挤出。压力单独控制粘土流动的速度，所以要得到正确的挤压速度有点挑剔。根据最终雕塑的大小，可以使用直径为 1 到 2 毫米的喷嘴。对于较大的作品，1 毫米的层高度效果很好。对于较小的片，0.5 毫米是优选的层高度。

这里使用的电子设备对于 3D 打印来说是非常标准的，一个带有斜坡屏蔽的 Arduino Mega。该固件是一个略有修改的马林变种。一个小问题被克服了，即使喷嘴没有被加热，发现 100K 热敏电阻仍然必须连接到斜坡板以保持固件满意。[Jonathan]已经将他所有构建文件、软件和固件放在他的页面上，供其他人用来制作他们自己的粘土打印机。

[https://www.youtube.com/embed/OOqAxePyJBg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/OOqAxePyJBg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

经由 [3D 打印机计划](http://3dprinterplans.info/tag/clay-3d-printer/)