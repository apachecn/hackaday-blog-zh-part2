# 一次品尝一种颜色的彩虹

> 原文：<https://hackaday.com/2014/12/14/taste-the-rainbow-one-color-at-a-time/>

康奈尔大学 Bruce Land 的 ECE4760 课程又一个秋季学期即将结束，这意味着基于微控制器的学生项目又有了新的收获。为了他们的项目，[爱丽丝、杰西和米哈伊尔]建造了一个彩虹糖分类微型工厂，将相同颜色的糖果装袋并密封成小小袋。

他们的设计分为三个阶段，在全纸板外壳内进行视觉描绘。彩虹糖被装入顶部的漏斗中，该漏斗通向颜色检测模块。颜色由 ATMega1284 驱动的 RGB LED 和 OPT101 光电二极管决定。因为红色和橙色彩虹糖的反射 RGB 值非常相似，所以探测器使用白光进行最终确定。

一旦匹配结束，第二阶段中的伺服旋转到与颜色结果相对应的角度。然后，彩虹糖滑下纸板滑槽，穿过纸板圆盘上的一个孔，落入一个悬挂的袋子中。一旦袋子达到预定的容量，另一个伺服移动袋的传送带到镍铬合金线密封装置。首席工厂工人[杰西]必须在这一点上进行干预，将袋子从生产线上拉下来。休息之后，您可以看到这个 Skittle 风味分离器的完整演示。

 [https://www.youtube.com/embed/AKqUffCPEWo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/AKqUffCPEWo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)